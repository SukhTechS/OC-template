# OC-template

OpenClaw deployment template — a pre-configured 5-agent AI team for rapid project setup.

## Quick Start

```bash
# Clone the template
git clone https://github.com/YOUR_ORG/OC-template.git my-project
cd my-project

# Customize agent names and config
# Edit each agent's SOUL.md, IDENTITY.md, USER.md

# Deploy with OpenClaw
openclaw deploy
```

## Agent Team

| Agent | Role |
|-------|------|
| **orchestrator** | Main command layer, workflow coordination |
| **db_agent** | Database ops, PostgreSQL, enrichment pipelines |
| **devops_agent** | Infrastructure, deployment, monitoring |
| **qa_agent** | Quality checks, data validation |
| **integrations_agent** | Third-party APIs, scraping, Chrome automation |

## Port Conventions

- **Dev**: 8889
- **Prod**: 8888

## Git Workflow

1. Work on `dev` branch
2. Test on port 8889
3. Push to `main` / production

## Customization Checklist

- [ ] Fill in agent SOUL.md with your company voice
- [ ] Update IDENTITY.md with agent names
- [ ] Set USER.md with company/team info
- [ ] Configure database credentials in db_agent/MEMORY.md
- [ ] Set timezone in USER.md files
- [ ] Add company-specific skills

## File Structure

```
OC-template/
├── AGENTS.md              # Agent roster
├── README.md              # This file
├── SOUL.md                # Workspace AI identity
├── IDENTITY.md            # Workspace name
├── USER.md                # Primary user info
├── HEARTBEAT.md           # Health check config
├── TOOLS.md               # Tool configuration
├── BOOTSTRAP.md           # First-run setup
├── orchestrator/          # Orchestrator agent
│   ├── SOUL.md
│   ├── IDENTITY.md
│   ├── USER.md
│   ├── TASK.md
│   └── MEMORY.md
├── db_agent/              # Database agent
├── devops_agent/          # DevOps agent
├── qa_agent/              # QA agent
└── integrations_agent/    # Integrations agent
```

## Notes

- Keep credentials in environment variables, never in code
- MEMORY.md files are agent-specific — keep generic in template
- SOUL.md defines personality — customize per company voice
