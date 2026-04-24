# AGENTS.md

## Agent Directories

Each agent has its own subdirectory with:
- TASK.md: Task definition
- MEMORY.md: Agent-specific memory
- SOUL.md: Agent personality (optional)
- Work files and scripts

## Agent List

- **orchestrator/** - Main orchestration agent
- **db_agent/** - Database operations
- **devops_agent/** - DevOps and infrastructure
- **qa_agent/** - Quality assurance
- **integrations_agent/** - Third-party integrations

## Git Workflow

1. Work on `dev` branch first
2. Test on port 8889
3. Then push to `main` / production (port 8888)
