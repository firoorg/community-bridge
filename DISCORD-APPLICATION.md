# Discord privileged-intent application

Discord application: **585765045800140812**  
Operator: **Firo Core Team**  
Public contact: **team@firo.org**

These answers reflect the two-way bridge and the user controls confirmed on 19 October 2026. The bot is installed in one Discord server.

## Application details

The application is Firo's official community chat bridge, operated by the Firo Core Team using self-hosted TediCross.

It connects our public Telegram community at https://t.me/firoorg with configured public channels in our official Discord server at https://discord.com/invite/TGZPRbRT3Y. It forwards ordinary community messages in both directions so people can participate in the same conversation from either platform.

The bridge processes message content, supported attachments, sender attribution and associated message and routing identifiers. Technical records support delivery, replies and the edit or deletion features available in the installed software. The bridge is used for community communication rather than advertising, profiling, AI training or a separate historical chat archive.

Our privacy and support contact is team@firo.org.

## Public privacy policy

Select **Yes** once the policy is publicly accessible and the community disclosure is in place.

Current repository URL:
https://github.com/firoorg/community-bridge/blob/main/docs/privacy.md

After GitHub Pages is enabled and deployment succeeds:
https://firoorg.github.io/community-bridge/privacy/

Terms:
https://firoorg.github.io/community-bridge/terms/

Open the actual URLs while logged out before submitting. The presence of the files does not mean Pages has deployed.

## Requested intents

Select **Message Content** for the two-way relay.

Do not also select Presence or Server Members for the basic message relay. If another enabled feature genuinely needs either intent, justify that feature separately and confirm the installed bot's gateway settings.

## Can users opt out of having their message content data tracked?

Select **No** for the currently confirmed setup.

There is currently no per-user forwarding opt-out. Users who do not want future forwarding should avoid posting in a bridged space. We accept manual deletion requests at team@firo.org and through official moderators. Deletion is separate from opting out of future processing.

Do not change this answer to Yes solely because users can leave a channel or request deletion of a past post.

## Are you storing message content data off-platform outside Discord?

Select **Yes**.

Discord posts and supported media are copied into the corresponding Telegram chat as the bridge's intended function. Telegram retains the destination posts under its platform operation and user/moderator controls.

The self-hosted relay also processes data during delivery and uses technical records such as message-ID mappings and delivery checkpoints. Diagnostic logs or other operational records may include information associated with messages and delivery failures. There is no separate intentional historical chat-archiving service. Our privacy policy describes retention and how users can request deletion; it does not claim that every record expires after 24 hours.

## Will content be used to train machine-learning or AI models?

Select **No**.

The Firo Core Team does not use bridge data to train machine-learning or AI models. This statement describes the operator's use of bridge data.

## Why do you need the Message Content intent?

The bridge must read ordinary messages in the configured public Firo Discord channels and forward their content and supported attachments to the linked official Telegram chat. Without Message Content access, the fields needed to relay ordinary channel messages can be empty, preventing the Discord-to-Telegram direction from working.

Requiring a slash command, message-context-menu action or bot mention for every post would require a separate manual action for each contribution and would not provide the ongoing two-way community conversation the bridge is designed to support.

We use the data to deliver the conversation, display sender attribution and support the reply, edit and deletion behavior available in the deployed software. Our public privacy policy explains the cross-platform sharing, operational records and manual deletion-request contact.

## Demonstration evidence

The form also requires real screenshot or video links. Create a short demonstration using posts you author:

1. Show the bridge disclosure and linked spaces.
2. Send an ordinary Discord message without mentioning the bot and show it arriving in Telegram.
3. Reply from Telegram and show it arriving in Discord.
4. Show media, replies or edit/deletion behavior only if it actually works in the deployment.

Paste the real accessible evidence URL into the form. No evidence URL is invented in this document.

## Operational preparation

Before submitting, introduce the community disclosure and establish the required user direction to forwarding. Check the server settings described in MAINTAINER-NOTES.md before giving any additional answers about exact retention or security. The upstream source does not establish the production server's version, encryption, log rotation or backup settings.
