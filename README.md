# UrbanismZK

A Quarto-based zettelkasten-style knowledge management system for urbanism and urban design, with structured notes, literature citations, and data visualizations.

## Structure

```
UrbanismZK/
├── _quarto.yml           # Quarto configuration
├── bibliography.bib      # BibTeX references
├── index.qmd            # Home page
├── primary/             # Primary notes with declarative titles
│   └── index.qmd        # Index of primary notes
├── aggregators/         # Topic-based collections of notes
│   └── index.qmd        # Index of aggregators
├── data/                # CSV files and datasets
├── templates/           # Templates for new notes
│   ├── primary-note-template.qmd
│   └── aggregator-note-template.qmd
└── styles.css           # Custom CSS styling
```

## Note Types

### Primary Notes

Located in `primary/`, these are declarative notes (e.g., "X causes Y") with structured sections:

- **Summary**: Concise overview of the main claim
- **Details**: In-depth explanation with evidence
- **Figures**: Data visualizations and graphics
- **See Also**: Links to related notes and aggregators

Primary notes cite literature using BibTeX citations (e.g., `@author2023`) and include a References section.

### Aggregator Notes

Located in `aggregators/`, these collect all primary notes related to a specific topic or theme. They provide:

- Overview of the topic
- Organized lists of related primary notes
- Key insights from examining notes together
- Links to related aggregators

### Data

Located in `data/`, this directory contains CSV files and raw datasets used for generating figures in notes.

## Getting Started

### Creating a New Primary Note

1. Copy `templates/primary-note-template.qmd` to `primary/`
2. Rename with a descriptive filename (use hyphens, e.g., `urban-density-reduces-emissions.qmd`)
3. Fill in the title, summary, details, and other sections
4. Add citations to `bibliography.bib` if needed
5. Update `primary/index.qmd` to link to your new note

### Creating a New Aggregator Note

1. Copy `templates/aggregator-note-template.qmd` to `aggregators/`
2. Rename with a topic name (e.g., `urban-emissions.qmd`)
3. Add links to relevant primary notes
4. Update `aggregators/index.qmd` to link to your new aggregator

### Adding Citations

Add BibTeX entries to `bibliography.bib`, then cite them in your notes using `@citationkey` syntax.

### Building the Site

```bash
quarto preview  # Preview with live reload
quarto render   # Build static site to _site/
```

## Tips

- Use descriptive, declarative titles for primary notes
- Link liberally between related notes
- Keep summaries concise (1-2 paragraphs)
- Use figures to illustrate key points
- Update aggregators as you add new primary notes
