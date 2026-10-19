---
layout: default
title: Privacy Policy
permalink: /privacy/
---

# Firo community bridge privacy policy

Effective date: 19 October 2026  
Last updated: 19 October 2026

## 1. Operator and scope

The **Firo Core Team**, an unincorporated group, operates the Firo community bridge and manages its relay server. In this policy, "we", "us" and "our" refer to the team operating that bridge.

For privacy questions and requests, contact **[team@firo.org](mailto:team@firo.org)**.

The bridge connects the [public Firo Telegram community at @firoorg](https://t.me/firoorg) with configured public channels in the [official Firo Discord server](https://discord.com/invite/TGZPRbRT3Y). This policy covers the bridge and its operational records. It does not govern the Firo blockchain, unrelated Firo services, or the independent services of Discord and Telegram.

## 2. Public messages and cross-platform forwarding

The bridge relays messages in both directions. A message in a bridged Discord channel can appear in Telegram, and a message in the linked Telegram chat can appear in Discord. Only the configured public spaces are forwarding destinations.

Forwarded content can include the message, supported media and displayed sender attribution. The destination may have a different audience, and participants may save, quote or redistribute what they can see. The bridge does not provide end-to-end encryption between the two platforms.

Public availability does not make information non-personal. Usernames, user IDs, profile details and the contents of a public post can still identify or concern a person. Please avoid posting information you do not want shared with the linked public community.

## 3. Information processed

The bridge uses TediCross to process the information needed for cross-platform conversation:

- Message text, captions, links and supported attachments, including images, audio, video, documents and stickers where relayed.
- Sender information supplied by the platforms, such as user IDs, usernames, display names or server nicknames, and profile images where used in message attribution.
- Routing and conversation metadata, including server, channel, chat, thread and message IDs, timestamps, reply references, and available edit or deletion events.
- Technical records needed for delivery and continuity, such as mappings between source and destination message IDs and the latest processed message.
- Diagnostic information, including errors, delivery failures and associated identifiers. Depending on the software and logging settings, diagnostics can include filenames, message excerpts or other information associated with a failed request.
- Information voluntarily supplied when someone emails us or asks moderators to handle a request.

The configured bridge relays public community conversations. It is not intended as a relay for private direct messages.

## 4. Purposes

We process this information to relay conversations, attribute posts, handle supported replies and updates, keep the bridge working, investigate failures, protect the service, moderate the linked communities and respond to requests.

We do not use bridge data for advertising, unrelated analytics or profiling, sale of data, training machine-learning or AI models, or a separate historical chat-archiving service. We do not intentionally forward it to additional services beyond those needed to provide the Discord and Telegram bridge.

The forwarding described here is the service offered to users of the linked spaces. Publication of this policy does not itself establish a user's consent or direction to share earlier messages, and it does not replace any authorization required by applicable law or platform rules.

## 5. Recipients and international processing

Relayed posts are shared with the destination platform and the people who can access the destination chat or channel. The platforms already hold the original posts submitted to them and receive the relayed copies delivered to their services.

Authorized Firo Core Team maintainers, and infrastructure providers needed to host and operate the relay, may process operational data for those purposes. We may also disclose information where required by law.

Discord, Telegram and infrastructure providers may process data in countries other than a participant's country. The bridge does not promise that all processing occurs in one country.

The platforms have their own terms, privacy policies, retention practices and user controls:

- [Discord Privacy Policy](https://discord.com/privacy)
- [Telegram Privacy Policy](https://telegram.org/privacy)

The website hosting these policies is served by GitHub Pages when enabled. GitHub may process visitors' technical information under the [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). The policy pages do not add an operator-run advertising or analytics service.

## 6. Storage and retention

The bridge's purpose is to relay a conversation. This still involves handling data outside the source platform and keeping technical records.

| Category | Retention and removal |
| --- | --- |
| Original and relayed posts on Discord or Telegram | Posts can remain in the relevant public conversation until removed through platform or moderator controls. Platform retention rules also apply. |
| Message and media data used during delivery | Data is processed through the relay software and its temporary runtime caches as needed to deliver messages and supported conversation context. It is not intentionally collected into a separate historical chat archive. |
| Message-ID mappings and delivery checkpoints | Technical records support replies, updates, continuity and recovery. They can be held in memory or written to disk, depending on configuration, and persisted records can survive restarts. |
| Diagnostics, logs and any system backups | Operational records may be retained by the relay server and its supporting systems. Logs can contain information associated with errors or delivery events. Backup copies, if made, can retain those records as well. |
| Email and moderation requests | Correspondence and a record of the action taken are kept only as needed to handle the request, necessary follow-up and any legal obligation. |

We do not currently promise a fixed automatic expiry period for message-ID records, server logs or backup copies. In particular, a software default for an in-memory mapping is not a guarantee that all records disappear after that period.

Our retention policy is to keep operator-held personal data only for the bridge's stated purposes and any applicable legal obligation, and to remove it when it is no longer necessary or a valid deletion requirement applies. You may request deletion of records within our possession or control using the contact below.

Expiry of a mapping or deletion of a local record does not remove a post already published on Discord or Telegram. Deleting a live record may also require separate handling of any retained backup copy. We handle deletion requirements for those copies as applicable; they are not an exception allowing unrelated reuse.

## 7. Choices and deletion requests

**There is currently no per-user forwarding opt-out.** To avoid future forwarding, do not post in a space that is being bridged. You may contact us to ask which spaces are linked or whether an alternative is available. Leaving a space does not remove posts already made.

You can email **[team@firo.org](mailto:team@firo.org)** or contact an official community moderator to request correction or deletion of a relayed post. Email is also available after leaving the community and for requests concerning other operator-held records.

Include the relevant platform, your username or user ID, and message links or approximate dates where possible. We may ask for proportionate information to verify that the request concerns your data. Please do not send account passwords, bot tokens or unrelated sensitive documents.

Requests are handled manually. We review them promptly, coordinate with moderators to remove relevant copies under our control, and address other retained operator-held data as required. If a particular action cannot be completed, we explain the limitation and available next steps. Applicable legal rights and response deadlines take precedence.

Do not assume that deleting a source message automatically deletes the forwarded copy. Synchronization depends on software support, settings, platform APIs and whether the relevant mapping remains available. A manual request can be made even after automatic synchronization is unavailable.

We cannot promise removal of copies independently saved by other participants, or information controlled solely by a platform. Those limitations do not remove our responsibility for data within our possession or control.

## 8. Security and privacy rights

The Firo Core Team administers the relay. Access for maintenance and request handling is limited to authorized maintainers and necessary service providers. Bot connections use platform authentication credentials. No system can guarantee absolute security, and public posts remain visible to their audiences.

If you suspect unauthorized access to bridge data, contact **team@firo.org**. We investigate and take appropriate remedial and notification steps under applicable requirements.

Depending on the law applicable to you and the processing, you may have rights to access, correct or delete personal data, object to or restrict processing, or complain to a relevant data-protection authority. Contact us to exercise an applicable right. This policy does not restrict mandatory legal protections.

## 9. Age requirements

The bridge is intended for people who meet the relevant platform's age requirements and applicable law. It is not directed to children below those requirements.

## 10. Changes and contact

We update this policy when the bridge or its data practices change and revise the date above. We provide appropriate notice of material changes as required. New destinations or data uses remain subject to applicable notice and authorization requirements.

**Firo Core Team**  
**[team@firo.org](mailto:team@firo.org)**

[Terms of Service]({{ '/terms/' | relative_url }}) · [Policy home]({{ '/' | relative_url }})
