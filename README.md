# RELIC
Repository for the ERC Starting Grant Project RELIC

## News Management
The news section of the RELIC website is populated dynamically from Markdown files stored in the `news/` folder of this repository.

### Adding News
To add a new news item, create a new `.md` file in the `news/` directory.

#### Formatting Requirements
For the frontend to correctly parse and display the news cards, follow this exact structure:

1.  **Title**: The first line should be the title wrapped in double asterisks.
    - Example: `**My News Title**`
2.  **Date**: The next relevant line should be the date in `yyyy.mm.dd` format, wrapped in single asterisks.
    - Example: `*2026.04.16*`
3.  **Content**: The rest of the file is the news content in standard Markdown.

#### Adding Images
1.  Store images in the `news/` folder (or a subfolder like `news/images/`).
2.  Reference them in your Markdown file using a relative path starting with `/news/`.
    - Example: `![image description](/news/images/my-image.jpg)`
    - *Note: The frontend automatically converts these paths to absolute GitHub URLs.*

### Example File Content
```markdown
**How does RELIC look at the Christianization of Europe?**

*2026.04.16*

This is the content of the news post. It can contain multiple paragraphs.

![image description](/news/images/ImageNews1.jpg "Mouseover text")

More content follows here...
```
