---
trigger: always_on
---

# dovi_convert documentation technical writing rule

## Project context

- This is a documentation project on the dovi_convert project
- The documentation for dovi_convert is in a separate repo: dovi_convert_docs, also added to this workspace
   - meaning:
   - Repo for the actual code: dovi_convert (folder in workspace: dovi_convert)
   - Repo for the user documentation: dovi_convert_docs (folder in workspace: dovi_convert_docs)
- IMPORTANT: This is user facing documentation, explaining users how to use dovi_convert. It is NOT internal documentation.
- We use Mintlify for documentation
- We use MDX files with YAML frontmatter  
- Navigation is configured in `docs.json`
- We follow technical writing best practices

## Writing standards

- Use second person ("you") for instructions
- Write in active voice and present tense
- Start procedures with prerequisites
- Include expected outcomes for major steps
- Use descriptive, keyword-rich headings
- Keep sentences concise but informative
- Avoid marketing speech and AI-slop at all cost. 
   - We are not trying to sell the tool
   - This is not a startup pitching a product to VCs
   - Do not invent and fancy feature names

## Required page structure

Every page must start with frontmatter:

```yaml
---
title: "Clear, specific title"
description: "Concise description for SEO and navigation"
---
```

## Mintlify components

### docs.json

- Refer to the [docs.json schema](https://mintlify.com/docs.json) when building the docs.json file and site navigation

### Callouts

- `<Note>` for helpful supplementary information
- `<Warning>` for important cautions and breaking changes
- `<Tip>` for best practices and expert advice  
- `<Info>` for neutral contextual information
- `<Check>` for success confirmations

### Code examples

- When appropriate, include complete, runnable examples
- Use `<CodeGroup>` for multiple language examples
- Specify language tags on all code blocks
- Include realistic data, not placeholders
- Use `<RequestExample>` and `<ResponseExample>` for API docs

### Procedures

- Use `<Steps>` component for sequential instructions
- Include verification steps with `<Check>` components when relevant
- Break complex procedures into smaller steps

### Content organization

- Use `<Tabs>` for platform-specific content
- Use `<Accordion>` for progressive disclosure
- Use `<Card>` and `<CardGroup>` for highlighting content
- Wrap images in `<Frame>` components with descriptive alt text

## API documentation requirements

- Document all parameters with `<ParamField>` 
- Show response structure with `<ResponseField>`
- Include both success and error examples
- Use `<Expandable>` for nested object properties
- Always include authentication examples

## Quality standards

- Use relative paths for internal links
- Include alt text for all images
- Ensure proper heading hierarchy (start with h2)
- Check existing patterns for consistency