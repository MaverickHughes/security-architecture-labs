# Current-State Email Security Architecture

## Business Context

The organization currently uses Barracuda Email Security Gateway as the primary secure email gateway for inbound and outbound email protection.

Microsoft 365 provides the underlying email platform.

## Current Mail Flow

Document the current mail path here.

Example:

Internet
→ Barracuda ESG
→ Microsoft 365 / Exchange Online
→ User Mailbox

Outbound:

User Mailbox
→ Microsoft 365 / Exchange Online
→ Barracuda ESG
→ Internet

## Security Controls

Document the controls currently provided by each platform.

### Barracuda ESG

- Spam filtering
- Malware filtering
- Phishing protection
- URL inspection
- Attachment inspection
- Policy enforcement
- Email continuity or quarantine features, if applicable

### Microsoft 365

- Exchange Online Protection
- Anti-spam controls
- Anti-malware controls
- Mail flow rules
- SPF
- DKIM
- DMARC
- Microsoft Defender capabilities currently enabled

## Dependencies

Document anything that depends on the current mail flow.

Examples:

- MX records
- SMTP connectors
- Transport rules
- Allowed sender lists
- IP allowlists
- Relay configuration
- Multifunction printers
- Internal applications
- Third-party SaaS platforms
- Journaling
- Archiving
- DLP
- Encryption
- Automated notifications

## Known Limitations

Document weaknesses or operational problems in the current design.

## Migration Constraints

Document anything that cannot break during migration.

Examples:

- Inbound mail delivery
- Outbound mail delivery
- Application relay
- Executive email
- Distribution lists
- Shared mailboxes
- External forwarding
- Partner mail flows
