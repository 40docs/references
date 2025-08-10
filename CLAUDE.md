# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the **references** repository - part of the 40docs platform's technical reference documentation collection. It contains comprehensive reference materials for Documentation as Code practices, MkDocs formatting, Git workflows, and platform architecture.

## Repository Structure

```
references/
├── index.md                    # Main reference index
├── docs-as-code.md            # Documentation as Code principles
├── others-using-dac.md        # Examples of DAC implementations
├── documentation-layout.md    # Content organization guidelines
├── FAQ.md                     # Frequently asked questions
├── git-reference.md           # Git workflow reference
├── md-reference.md           # Markdown syntax reference
├── mkdocs/                   # MkDocs-specific formatting guides
│   ├── index.md
│   ├── admonitions.md        # Callout boxes and alerts
│   ├── annotations.md        # Interactive annotations
│   ├── buttons.md           # Button styling
│   ├── code-blocks.md       # Code syntax highlighting
│   ├── content-tabs.md      # Tabbed content
│   ├── data-tables.md       # Table formatting
│   ├── diagrams.md          # Mermaid and other diagrams
│   ├── embedding-external-files.md
│   ├── formatting.md        # Text formatting
│   ├── grids.md            # Layout grids
│   ├── icons-emojis.md     # Icon and emoji usage
│   ├── images.md           # Image handling
│   ├── lists.md            # List formatting
│   └── tooltips.md         # Interactive tooltips
└── assets/
    └── images/             # Reference images and screenshots
```

## Content Guidelines

### Writing Style
- **Technical Accuracy**: All code examples must be tested and functional
- **Clear Examples**: Include practical examples for each concept
- **Consistent Formatting**: Follow MkDocs Material theme conventions
- **User-Focused**: Write for developers and technical writers who need quick reference

### MkDocs Reference Content
The `mkdocs/` directory contains comprehensive formatting guides for:
- **Visual Elements**: Admonitions, buttons, grids, icons
- **Interactive Features**: Annotations, content tabs, tooltips  
- **Technical Content**: Code blocks, diagrams, data tables
- **Media Integration**: Images, embedded files

### Documentation Standards
- Use frontmatter for navigation and metadata
- Include practical code examples in all technical guides
- Test all MkDocs syntax examples before committing
- Maintain consistent voice and structure across guides

## Development Commands

### Content Validation
```bash
# Install MkDocs for local testing (if available)
pip install mkdocs mkdocs-material

# Preview content locally (from parent directory with mkdocs.yml)
mkdocs serve

# Validate Markdown syntax
markdownlint **/*.md
```

### Git Workflow
```bash
# Create content branch
git checkout -b content/new-reference-topic

# Add new reference material
git add .
git commit -m "docs: add reference guide for [topic]"

# Push for review
git push origin content/new-reference-topic
```

## Content Types

### Reference Documentation
- **Syntax Guides**: Markdown and MkDocs formatting reference
- **Code Examples**: Practical implementation examples  
- **Best Practices**: Proven patterns and approaches
- **Troubleshooting**: Common issues and solutions

### MkDocs Formatting Examples
Each guide in `mkdocs/` demonstrates:
- Syntax for the specific feature
- Visual examples of rendered output
- Common use cases and variations
- Integration with MkDocs Material theme

## Important Notes

### Multi-Repository Context
- This is a submodule of the larger 40docs platform
- Content here is referenced by multiple documentation sites
- Changes may affect multiple downstream repositories
- Follow Documentation as Code principles outlined in `docs-as-code.md`

### Content Dependencies  
- Images in `assets/images/` are referenced across multiple guides
- MkDocs examples assume Material theme extensions
- Code examples should work with the platform's MkDocs configuration

### Quality Standards
- All formatting examples must render correctly in MkDocs Material
- Code blocks must include appropriate language syntax highlighting  
- Screenshots should be current and match the described functionality
- External links should be verified and current

## Testing Guidelines

### Local Testing
- Test MkDocs syntax changes in a local MkDocs environment
- Verify image references and links resolve correctly
- Check that code examples are syntactically correct
- Validate frontmatter YAML syntax

### Content Review
- Ensure new content follows existing style and structure
- Verify technical accuracy of all examples
- Test that formatting renders correctly across different screen sizes
- Check accessibility of content (headings, alt text, etc.)

This repository serves as the definitive reference for Documentation as Code practices within the 40docs ecosystem. Content should be comprehensive, accurate, and immediately useful to developers and technical writers.