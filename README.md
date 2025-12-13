# Portfolio Case Study Site

A portfolio website built with Astro + MDX for showcasing case studies with a consistent layout and typographic structure.

## Features

- **Astro + MDX** for fast, static case study pages
- **Component-based layouts** with reusable components
- **Easy color customization** via CSS variables

## Getting Started

```bash
npm install
npm run dev
```


## Creating a New Case Study

1. Duplicate `src/content/stories/case-study-template.mdx`
2. Rename it (e.g., `my-project.mdx`)
3. Update the frontmatter (title, lede, meta, sections)
4. Write your content using the section structure
5. Use components: `<PullQuote />`, `<Callout />`, `<MetricsGrid />`

## Customization

Edit `public/styles/case-study.css` to customize:
- Colors (CSS variables at the top)
- Typography scale
- Spacing and layout
- Component styles

## Components Usage

### PullQuote
```mdx
<PullQuote 
  quote="Your quote here"
  attribution="Author name"
/>
```

### Callout
```mdx
<Callout title="Optional Title">
  <p>Your callout content here.</p>
</Callout>
```

### MetricsGrid
```mdx
<MetricsGrid 
  metrics={[
    { value: "42%", label: "Increase in engagement" },
    { value: "3.2x", label: "Faster load times" }
  ]}
/>
```
