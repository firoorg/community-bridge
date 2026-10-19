# Firo community bridge

Policies and notices for the official two-way bridge between Firo's public Telegram community and configured public channels in its Discord server.

Operator: **Firo Core Team**, an unincorporated group.  
Contact: **team@firo.org**  
Discord application ID: **585765045800140812**

## Policies

- [Privacy Policy](docs/privacy.md)
- [Terms of Service](docs/terms.md)
- [Bridge notice to post in both communities](BRIDGE-NOTICE.md)
- [Discord intents application answers](DISCORD-APPLICATION.md)
- [Maintainer notes and source findings](MAINTAINER-NOTES.md)

## Enable GitHub Pages

The public pages are in `docs/`.

1. Open [Settings > Pages](https://github.com/firoorg/community-bridge/settings/pages).
2. Under Build and deployment, choose **Deploy from a branch**.
3. Select **main**, choose **/docs**, and save.
4. Wait for GitHub's deployment to finish and check the published pages while logged out.

With the repository's current organization and name, the addresses will be:

- https://firoorg.github.io/community-bridge/
- https://firoorg.github.io/community-bridge/privacy/
- https://firoorg.github.io/community-bridge/terms/

The pages become available after Pages is enabled and deployment succeeds. Add the live privacy and terms URLs to the corresponding fields in Discord's Developer Portal.

## Community notice and requests

Post the notice in both communities, including each bridged Discord channel's description or a prominent pinned message. The notice describes cross-platform forwarding and links to the policies.

Public messages can contain personal data. The email contact accepts privacy and deletion requests even though the bridged conversations are public. Moderators can remove relayed messages manually. There is currently no per-user forwarding opt-out.

Before continuing forwarding after introducing the disclosure, establish clear user direction to the cross-platform sharing. A posted policy alone does not demonstrate the express user direction Discord requires. See the maintainer notes.

## Maintaining these policies

The policies use the operator's confirmed facts and account for the upstream software's technical records. They do not claim a verified server location, a particular installed version, a fixed log/backup expiry, encryption at rest, or an opt-out feature that has not been established.

Confirm the deployed configuration and keep the policy accurate when data handling changes. The repository contains no bot credentials, production configuration, chat logs or private user records.
