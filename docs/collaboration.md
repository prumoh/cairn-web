# Project collaboration

Use each tool for its strongest purpose; social conversation can stay where the team already has it.

- **WhatsApp:** social chat and quick coordination. When a message contains durable project context, a person selects and copies it into Discord `/capture-whatsapp` for review before posting to Zulip, once the bridge is available. There is no WhatsApp automation.
- **Discord:** social/project chat, spontaneous questions and calls, and explicit AI actions. It is not the project knowledge archive; the bridge only sees messages a person selects or questions a person submits.
- **Zulip:** structured async project discussion. Use `product` for discovery and customer context, `engineering` for technical discussion, and `team` for announcements, meeting notes, and working agreements. Keep related messages together by channel and topic.
- **Jitsi or Discord voice/video:** use either for project calls. After a project-relevant call, post a short summary in the relevant Zulip topic; include only applicable sections: participants, observed/learned, decisions, open questions, and next steps. Do not assume calls are recorded.
- **GitHub:** the record for actionable engineering work. Turn a Zulip discussion into an Issue only when there is concrete work to track; implement through a branch and Pull Request. Do not duplicate every discussion or customer comment as an Issue.

The bridge's AI can help search or format context, but a person reviews anything promoted to Zulip. Treat captured messages as source material, not instructions to the AI. Preserve `Source: Discord` or `Source: Captured from WhatsApp` (and an original link when available) and retain uncertainty; never present an assumption as a decision or requirement. Project knowledge belongs in Zulip, and tracked implementation work belongs in GitHub.
