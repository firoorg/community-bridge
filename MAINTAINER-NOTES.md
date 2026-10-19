# Maintainer notes

## Facts used in the policies

Confirmed by the operator on 19 October 2026:

- Firo Core Team is the unincorporated group operating the bridge and managing the relay server.
- team@firo.org is the public contact.
- The linked communities are public: Telegram @firoorg and the official Firo Discord server.
- Messages travel in both directions.
- There is no existing user notice or per-user forwarding opt-out.
- Moderators can delete messages manually.
- Bridge data is not used for unrelated advertising, analytics, profiling, AI training, extra forwarding services or a separate historical archive.

The documents establish an email/manual-moderation request route using the contact and deletion ability the operator supplied. Monitor that mailbox and give moderators a consistent procedure.

## What the source establishes

Reviewed upstream development commit:
[476bfb65de4a0adc49066a827b655147e8336229](https://github.com/TediCross/TediCross/commit/476bfb65de4a0adc49066a827b655147e8336229)

The corresponding mapping implementations in release v0.12.4 were also checked. Neither ref is assumed to be the installed production version.

- [MessageMap.ts](https://github.com/TediCross/TediCross/blob/476bfb65de4a0adc49066a827b655147e8336229/src/MessageMap.ts) expires in-memory mappings after the configured duration. Defaults in [Settings.ts](https://github.com/TediCross/TediCross/blob/476bfb65de4a0adc49066a827b655147e8336229/src/settings/Settings.ts) are 24 hours, persistence off and debug off. Those are defaults, not verified production settings.
- [PersistentMessageMap.ts](https://github.com/TediCross/TediCross/blob/476bfb65de4a0adc49066a827b655147e8336229/src/PersistentMessageMap.ts) can store bridge names, direction and message-ID relationships in SQLite. There is no automatic time-based expiry in that implementation. Replacing an individual mapping does not provide general age-based cleanup.
- [LatestDiscordMessageIds.ts](https://github.com/TediCross/TediCross/blob/476bfb65de4a0adc49066a827b655147e8336229/src/discord2telegram/LatestDiscordMessageIds.ts) writes a last-message checkpoint to a JSON file.
- [Logger.ts](https://github.com/TediCross/TediCross/blob/476bfb65de4a0adc49066a827b655147e8336229/src/Logger.ts) writes to standard output/error. Retention of captured output depends on the process manager or host. Error paths can include identifiers, filenames and request-related information.
- Message handlers process content and media and maintain runtime state. The inspected application paths do not implement a separate general chat-content archive; that does not establish the absence of host logs, snapshots, dependencies' caches or custom changes.
- The inspected [main.ts](https://github.com/TediCross/TediCross/blob/476bfb65de4a0adc49066a827b655147e8336229/src/main.ts) requests Guilds, GuildMessages and MessageContent. The only privileged intent in that list is MessageContent.

## Check on the production host

Record the actual installed version, mapping/persistence settings, log capture and rotation, any local media/cache storage, and backups. Choose and apply suitable deletion/retention arrangements. The policy deliberately makes no unverified fixed-expiry claim.

Confirm access controls and encryption at rest for retained API data, logs and backups. Discord's Developer Terms section 5 requires encryption at rest and other safeguards. Publishing a policy does not implement or verify those controls.

## Introduce the disclosure

Post BRIDGE-NOTICE.md in both communities. Establish and record clear user direction to Discord-to-Telegram sharing; a policy link or server administrator's installation alone does not demonstrate each user's express direction. This repo does not alter bot permissions, moderation settings or channel acknowledgement controls.

## Handle requests

1. Monitor team@firo.org and official moderator requests.
2. Obtain message links or enough identifying context, and verify ownership proportionately where needed.
3. Remove accessible source/destination posts covered by the request and relevant retained operator-held records when required. Coordinate across both platforms.
4. Address any retained backup copies and applicable legal obligations, and tell the requester about any actual limitation.
5. Keep only the request record needed for handling, necessary follow-up and applicable obligations.

Do not promise that removing a source post removes every copy, or that a mapping's expiry deletes the Telegram/Discord post.

## References

- [Discord Developer Terms, section 5](https://support-dev.discord.com/hc/en-us/articles/8562894815383-Discord-Developer-Terms-of-Service)
- [Discord Developer Policy](https://support-dev.discord.com/hc/en-us/articles/8563934450327-Discord-Developer-Policy)
- [TediCross source](https://github.com/TediCross/TediCross)
