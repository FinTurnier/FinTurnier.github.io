# Finly Turnier — Portfolio Website

Personal portfolio for **Finly Turnier**, built as a static Jekyll site and
published through GitHub Pages. The repository also contains a separate Django
playground used for dynamic-application experiments.


**Live site:** https://finturnier.github.io

## Technology

### Public portfolio

- Jekyll with the `github-pages` gem
- Markdown and YAML front matter
- Liquid layouts and includes
- Hand-written CSS in `assets/css/style.css`
- GitHub Pages hosting
- GoatCounter privacy-first analytics
- Docker for the Ruby/Jekyll toolchain; local Ruby is not required

### Django playground

- Django 5.2.6
- PostgreSQL
- Pillow for image uploads
- Separate from the public static deployment; not currently published

## Repository map

```text
Portfolio-website/
├── README.md                     # This reference document
├── requirements.txt              # Python dependencies for the Django app
├── completion_reports/           # Local, gitignored completion reports
└── portfolio-project/
    ├── _config.yml               # Jekyll, deployment, and analytics config
    ├── Gemfile / Gemfile.lock    # Ruby dependencies
    ├── Dockerfile                # Jekyll image with gems installed
    ├── docker-compose.yml        # Local build and preview services
    ├── init.sh                   # Standard startup and baseline verification
    ├── publish.sh                # Verified static-only deployment
    ├── index.md                  # Homepage
    ├── about.md                  # About page
    ├── resume.md                 # Resume page
    ├── timeline.md               # Timeline page
    ├── projects.md               # Project index
    ├── notes.md / lessons.md     # Writing indexes
    ├── _projects/                # Portfolio project entries
    ├── _notes/                   # Working notes
    ├── _lessons/                 # Retrospectives and generalizable lessons
    ├── _data/timeline.yml        # Career timeline source of truth
    ├── _data/skills.yml          # Grouped skills used by About and Resume
    ├── _layouts/                 # Shared page layouts
    ├── _includes/                # Header, footer, cards, timeline
    ├── assets/css/style.css      # Theme and design tokens
    ├── AGENTS.md                 # Agent workflow and content rules
    ├── feature_list.json         # Feature status and verification evidence
    ├── claude-progress.md        # Session history and current state
    ├── jobs/                     # Django app
    ├── portfolio/                # Django settings and URLs
    └── manage.py                 # Django management entry point
```

## Prerequisites

For the normal portfolio workflow:

- Docker with the Compose plugin
- Git
- GitHub CLI (`gh`), authenticated as `FinTurnier`, for publishing

For Django development:

- Python 3
- PostgreSQL running locally or at a configured host
- Python dependencies from `requirements.txt`

No local Ruby, Bundler, or Jekyll installation is needed.
