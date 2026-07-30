# Privacy Policy for Corvax AHelp Discord Bot

**Effective date:** July 26, 2026  
**Last updated:** July 30, 2026

## 1. Overview

Corvax AHelp Discord Bot (the "Bot") is a moderation and player-support integration that connects administrator-help conversations on participating game servers with designated Discord channels and threads.

This Privacy Policy explains what information the Bot processes, why it is processed, where it is sent, and the choices available to users.

## 2. Information We Process

The Bot may process the following information:

- Discord user IDs, usernames, and display names of staff members who use the Bot;
- interaction data intentionally supplied to the Bot's `/ckey`, `/ah`, `/lso`, and `/reply` application commands;
- Discord server, channel, thread, message, and webhook identifiers needed to route an AHelp conversation;
- game-related information returned by a connected game server when an authorized staff member uses a command, such as player identifiers, connection status, character names, jobs, roles, or in-game objectives;
- AHelp conversation metadata supplied by connected game servers, including conversation identifiers, player identifiers, character names, server names, round identifiers, and conversation state.

The Bot does not request Discord's Message Content Intent, subscribe to message events, or inspect ordinary messages posted in channels or threads. It processes text only when a user explicitly supplies it as an application-command option. It does not download message attachments for these functions.

## 3. Where the Bot Processes Messages

The Bot accepts application-command interactions only in Discord channels explicitly configured for AHelp operation and in the AHelp threads associated with those channels. It does not process ordinary channel messages, direct messages, or messages in unrelated channels.

The Bot does not continuously profile Discord users or use message content for advertising or behavioral analytics.

## 4. How We Use Information

Information is processed only as needed to:

- recognize and execute authorized AHelp commands;
- create, identify, and route AHelp threads;
- relay a staff member's Discord reply to the corresponding in-game AHelp conversation;
- display game-server information requested by authorized moderation staff;
- operate, secure, troubleshoot, and prevent abuse of the AHelp service.

Message content and other user data are not sold and are not used to train machine-learning or artificial-intelligence models.

## 5. Sharing and External Processing

Text intentionally submitted to an AHelp conversation may be transmitted from Discord to the applicable Corvax game server through its restricted administrator-help API. Necessary Discord identifiers and the staff member's display name may accompany the message so that the game server can attribute and route it correctly.

Information may therefore be accessible to authorized Corvax administrators and to service providers that host Discord, the Bot, or the connected game servers. We do not share this information with third parties for advertising or data-broker purposes.

## 6. Storage and Retention

The Bot does not maintain its own persistent message-content database. It keeps current routing and conversation state temporarily in memory while the Bot is running.

Messages remain stored by Discord according to the settings and retention behavior of the relevant Discord server. Messages relayed to a game server may also be retained in restricted administrative or AHelp records for moderation, safety, abuse investigation, and audit purposes. Those records are retained only for as long as reasonably necessary for those purposes or as required by applicable obligations.

## 7. User Choices and Requests

The Bot does not track ordinary Discord messages. Users can avoid submitting data to the Bot by not invoking its application commands. There is no per-command opt-out after text has been intentionally submitted through `/ah` or `/reply` because processing that text is necessary to deliver the AHelp service.

Users may request access to or deletion of data controlled by the Corvax community by contacting the administrators of the Discord server where the Bot is installed. Please do not include sensitive personal information in a public support request. Some information may be retained when reasonably necessary for security, abuse prevention, record integrity, or legal compliance.

Users can independently delete their Discord messages where Discord permissions allow. Deleting a Discord message may not automatically delete an administrative record that was already relayed to a connected game server.

## 8. Security

We use reasonable technical and organizational safeguards intended to restrict access to AHelp data. These include limiting the Bot to configured channels, restricting administrative channels through Discord permissions, and authenticating communication with connected game servers. No method of electronic transmission or storage is completely secure.

## 9. Children's Privacy

The Bot is not directed to children below the minimum age required to use Discord in their country. We do not knowingly use the Bot to collect personal information from anyone who is not permitted to use Discord.

## 10. Changes to This Policy

We may update this Privacy Policy when the Bot's functionality or data practices change. The current version will be published at the same public URL, and the "Last updated" date will be revised.

## 11. Contact

For privacy questions or requests, contact the administrators of the Discord server where Corvax AHelp Discord Bot is installed through that server's official support or administration channel.
