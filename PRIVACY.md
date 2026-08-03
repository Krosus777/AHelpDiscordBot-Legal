# Privacy Policy for Corvax AHelp Discord Bot

**Effective date:** July 26, 2026  
**Last updated:** August 3, 2026

## 1. Overview

Corvax AHelp Discord Bot and its associated moderation-audit service (together, the "Service") connect administrator-help conversations on participating game servers with designated Discord channels and threads and produce restricted moderation activity statistics.

This Privacy Policy explains what information the Service processes, why it is processed, where it is sent, and the choices available to users.

## 2. Information We Process

The Service may process the following information:

- Discord user IDs, usernames, and display names of people whose messages appear in configured moderation or AHelp channels and threads;
- Discord role identifiers and role names used to verify command and dashboard access and to classify current staff roles;
- interaction data intentionally supplied to the Bot's `/ckey`, `/ah`, `/lso`, and `/reply` application commands;
- Discord server, channel, thread, message, and webhook identifiers needed to route an AHelp conversation;
- message timestamps, authorship and thread metadata from configured moderation channels, used to produce moderation activity statistics;
- AHelp webhook text and embed fields, processed temporarily to attribute staff responses and produce aggregate statistics;
- game-related information returned by a connected game server when an authorized staff member uses a command, such as player identifiers, connection status, character names, jobs, roles, or in-game objectives;
- AHelp conversation metadata supplied by connected game servers, including conversation identifiers, player identifiers, character names, server names, round identifiers, and conversation state.

The Service does not open a separate Discord Gateway connection for the moderation audit or subscribe that audit to message events. The audit reads configured channels and threads through Discord's official REST API. Under the current implementation, it discards the body, embeds, and attachment names of newly read ordinary moderation messages before persistence. AHelp webhook text is parsed in memory and then discarded; only the classification result and service metadata are newly persisted.

## 3. Where the Bot Processes Messages

The Bot accepts application-command interactions only in Discord channels explicitly configured for AHelp operation and in the AHelp threads associated with those channels. The associated audit reads only explicitly configured moderation and AHelp channels and their threads. It does not audit direct messages or unrelated Discord channels.

The Service does not continuously profile Discord users or use message content for advertising or behavioral analytics.

## 4. How We Use Information

Information is processed only as needed to:

- recognize and execute authorized AHelp commands;
- create, identify, and route AHelp threads;
- relay a staff member's Discord reply to the corresponding in-game AHelp conversation;
- display game-server information requested by authorized moderation staff;
- synchronize current staff roles and control access to the restricted moderation dashboard;
- produce aggregate moderation activity statistics;
- operate, secure, troubleshoot, and prevent abuse of the AHelp service.

Message content and other user data are not sold and are not used to train machine-learning or artificial-intelligence models.

## 5. Sharing and External Processing

Text intentionally submitted to an AHelp conversation may be transmitted from Discord to the applicable Corvax game server through its restricted administrator-help API. Necessary Discord identifiers and the staff member's display name may accompany the message so that the game server can attribute and route it correctly.

Information and aggregate moderation statistics may therefore be accessible to authorized Corvax administrators and to service providers that host Discord, the Service, or the connected game servers. We do not share this information with third parties for advertising or data-broker purposes.

## 6. Storage and Retention

The Bot keeps current routing and conversation state temporarily in memory while it is running. The current moderation audit persistently stores service metadata and aggregate results, such as Discord identifiers, timestamps, thread and channel identifiers, author identity, current role classification, whether an AHelp response was counted, and the reason for that classification. Newly processed ordinary message bodies, AHelp transcript text, webhook payloads, embeds, and attachment names are not written to the audit database.

The primary moderation database currently has no automatic fixed deletion schedule. Routine SQLite backups are normally rotated after 14 days. Operational records may be retained longer when reasonably necessary for security, abuse investigation, record integrity, or legal compliance.

Messages remain stored by Discord according to the settings and retention behavior of the relevant Discord server. Messages relayed to a game server may also be retained in restricted administrative or AHelp records for moderation, safety, abuse investigation, and audit purposes. Those records are retained only for as long as reasonably necessary for those purposes or as required by applicable obligations.

## 7. User Choices and Requests

Users can avoid submitting command data to the Bot by not invoking its application commands. Participation in configured moderation or AHelp channels may still result in the processing of message metadata and aggregate activity described above. There is no per-command opt-out after text has been intentionally submitted through `/ah` or `/reply` because processing that text is necessary to deliver the AHelp service.

Users may request access to or deletion of data controlled by the Corvax community by contacting the administrators of the Discord server where the Bot is installed. Please do not include sensitive personal information in a public support request. Some information may be retained when reasonably necessary for security, abuse prevention, record integrity, or legal compliance.

Users can independently delete their Discord messages where Discord permissions allow. Deleting a Discord message may not automatically delete already stored audit metadata or an administrative record that was relayed to a connected game server.

## 8. Security

We use reasonable technical and organizational safeguards intended to restrict access to AHelp and moderation-audit data. These include limiting processing to configured channels, restricting administrative channels and the moderation dashboard, authenticating communication with connected game servers, and limiting access to the operational database and backups. No method of electronic transmission or storage is completely secure.

## 9. Children's Privacy

The Bot is not directed to children below the minimum age required to use Discord in their country. We do not knowingly use the Bot to collect personal information from anyone who is not permitted to use Discord.

## 10. Changes to This Policy

We may update this Privacy Policy when the Bot's functionality or data practices change. The current version will be published at the same public URL, and the "Last updated" date will be revised.

## 11. Contact

For privacy questions or requests, contact the administrators of the Discord server where Corvax AHelp Discord Bot is installed through that server's official support or administration channel.
