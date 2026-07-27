# Cursor Agent Skills

Personal collection of Cursor agent skills — specialized capabilities that extend what the AI agent can do in the IDE.

## Structure

```
cursor-skills/
│
├── cursor-ide/          # Cursor-specific IDE workflow skills
│   ├── automate/        # Create Cursor Automations
│   ├── babysit/         # Keep a PR merge-ready in a loop
│   ├── canvas/          # Create live React canvas apps
│   ├── create-hook/     # Create Cursor hooks
│   ├── create-rule/     # Create persistent Cursor rules
│   ├── create-skill/    # Author new skills
│   ├── loop/            # Run a prompt on a recurring interval
│   ├── review-bugbot/   # Code review via Bugbot subagent
│   ├── review-security/ # Security review subagent
│   ├── sdk/             # Build apps on the Cursor SDK
│   ├── split-to-prs/    # Split work into small reviewable PRs
│   ├── statusline/      # Configure custom CLI status line
│   └── update-cursor-settings/ # Modify Cursor/VSCode settings
│
├── od-contribute/       # Open Design contribution flow (docs, i18n, skills, design systems)
│
├── ponytail/            # Lazy senior dev mode — forces minimal solutions
├── ponytail-audit/      # Whole-repo over-engineering audit
├── ponytail-debt/       # Harvest ponytail: debt comments into a ledger
├── ponytail-gain/       # Show ponytail's measured impact scoreboard
├── ponytail-help/       # Quick-reference card for all ponytail commands
├── ponytail-review/     # Code review focused on over-engineering
│
├── artifacts-builder/   # Multi-component Claude.ai HTML artifacts
├── brand-guidelines/    # Anthropic brand colors and typography
├── canvas-design/       # Visual art in .png and .pdf
├── changelog-generator/ # User-facing changelogs from git commits
├── competitive-ads-extractor/ # Extract and analyze competitor ads
├── connect/             # Connect Claude to external apps
├── connect-apps/        # Gmail, Slack, GitHub integrations
├── content-research-writer/   # Research-backed content writing
├── developer-growth-analysis/ # Analyze coding patterns and growth
├── docx/                # Word document creation and editing
├── domain-name-brainstormer/  # Domain name ideas + availability check
├── file-organizer/      # Intelligent file organization
├── image-enhancer/      # Image quality enhancement
├── internal-comms/      # Internal communications templates
├── invoice-organizer/   # Invoice and receipt organization
├── langsmith-fetch/     # Debug LangChain agents via LangSmith
├── lead-research-assistant/   # High-quality lead research
├── mcp-builder/         # Create MCP servers
├── meeting-insights-analyzer/ # Meeting transcript analysis
├── od-memory/           # Open Design daemon memory operations
├── pdf/                 # PDF manipulation toolkit
├── pptx/                # PowerPoint creation and editing
├── raffle-winner-picker/      # Random winner selection
├── skill-creator/       # Guide for creating new skills
├── skill-share/         # Create and share skills on Slack
├── slack-gif-creator/   # Animated GIFs for Slack
├── tailored-resume-generator/ # Job-tailored resume generation
├── template-skill/      # Skill template to start from
├── theme-factory/       # Style artifacts with preset themes
├── twitter-algorithm-optimizer/ # Optimize tweets for reach
├── video-downloader/    # Download YouTube videos
├── webapp-testing/      # Test local web apps with Playwright
└── xlsx/                # Spreadsheet creation and analysis
```

## How to use

Skills are picked up automatically by the Cursor agent when placed in `~/.cursor/skills/`. The agent reads the `SKILL.md` in each folder to understand when and how to invoke the skill.

To trigger a skill manually, type `/skill-name` in the chat (e.g. `/ponytail`, `/canvas`, `/changelog-generator`).

## Adding a new skill

1. Create a folder with a `SKILL.md` describing the skill's purpose and instructions.
2. Add any supporting scripts, templates, or reference docs inside the folder.
3. Commit and push to keep this repo in sync.
