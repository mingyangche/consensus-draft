# WMDC Consensus

> 🧘 World Meditation Day Consensus Platform

## About WMDC

The **World Meditation Day Consensus (WMDC)** is a collaborative platform for community-driven decision-making through meditation and mindful dialogue.

### Our Principles

- 🤝 **Collective Stillness** - Quiet presence creates space for wisdom
- 👥 **Inclusive Dialogue** - Every voice matters in our consensus process  
- 🐢 **Gentle Progress** - We move at a pace that honors all participants
- 📖 **Transparent Process** - All decisions and their rationale are openly documented

## Quick Start

### Local Development

```bash
# Clone the repository
git clone https://github.com/mingyangche/consensus-draft.git
cd consensus-draft

# Install Hugo (if not installed)
# macOS: brew install hugo
# Linux: sudo apt-get install hugo

# Preview the site
cd docs && hugo server
```

### View Online

The website is automatically deployed via GitHub Pages:
- **URL**: https://mingyangche.github.io/consensus-draft/

## Project Structure

```
.
├── .github/
│   └── workflows/          # GitHub Actions workflows
│       ├── deploy.yml       # Automatic deployment
│       └── test.yml         # Testing and validation
├── docs/                   # Hugo website files
│   ├── content/            # Page content (Markdown)
│   │   └── posts/          # Blog posts
│   ├── themes/             # Hugo themes
│   │   └── hugo-wmdc/      # Custom WMDC theme
│   └── config.toml         # Hugo configuration
└── README.md               # This file
```

## Contributing

We welcome contributions from meditators, facilitators, and community builders!

### How to Contribute

1. **Fork the Repository** - Create your own copy
2. **Create a Branch** - `git checkout -b feature/your-feature`
3. **Make Changes** - Edit content or code
4. **Test Locally** - Run `hugo server` to preview
5. **Submit a Pull Request** - We'll review together

## Automation & CI/CD

### Automated Tests

Every pull request triggers our test workflow:
- Project structure verification
- YAML syntax validation

### Automatic Deployment

On merge to `main`:
1. Hugo builds the static site
2. Deploys to GitHub Pages
3. Updates the live website

## Consensus Process

Learn about our decision-making approach:

1. **Intention Setting** - Define the question
2. **Silent Reflection** - Meditate on the matter
3. **Open Dialogue** - Share perspectives
4. **Sense Gathering** - Identify agreement
5. **Synthesis** - Create proposals
6. **Confirmation** - Verify acceptance

## Resources

- [Documentation](docs/content/)
- [GitHub Discussions](https://github.com/mingyangche/consensus-draft/discussions)
- [Issue Tracker](https://github.com/mingyangche/consensus-draft/issues)

## License

This project is open source. See [LICENSE](LICENSE) for details.

---

*In stillness, we find strength. In consensus, we find peace.*

🌍 Built with 🙏 by the WMDC Community
