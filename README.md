# Technology Radar Example

This is based on the [PagoPA technology radar](https://github.com/pagopa/technology-radar) ([see example here](https://pagopa.github.io/technology-radar/index.html))
 which is based on [AOE technology radar](https://github.com/AOEpeople/aoe_technology_radar).


## Content Guidelines

In order to add new content to the radar,
please follow these guidelines.

Place new Markdown content inside the `radar` directory,
one Markdown file for each technology/pattern.

Start every `.md` file with a frontmatter header ie.

```md
---
title: "Turborepo"
ring: trial
quadrant: "tools"
tags: [build, frontend]
---
```

| Key       | Possible values                                                                           |
| --------- | ----------------------------------------------------------------------------------------- |
| Tags      | cloud, java, javascript, typescript, mobile, web, api, backend, frontend, aws, azure, ... |
| Rings     | adopt, trial, assess, hold                                                                |
| Quadrants | tools, methods-and-patterns, languages-and-frameworks, platforms-and-aoe-services         |

When a pull request is merged into the `main` branch
the radar is automatically updated triggering a [GitHub Action](./.github/workflows/main.yml).

## Local development

To start local development, install the necessary dependencies
then start the development server:

```bash
npm install
npm run start
```

Finally, open the radar here: http://localhost:8080/

### Update content and UI

If you add new content to the radar directory,
you may need to regenerate the `rd.json` file.
You can do this while the server is running:

```
npm run generateJson
```

## Support

If you have any questions or suggestions, please use
the [discussion forum on GitHub](https://github.com/pagopa/technology-radar/discussions).

## Fonts

This tech-radar uses the [Roboto](https://fonts.google.com/specimen/Roboto) Google font family.

## Site Logo
The site logo was created with an SVG free online creator, [svgator](https://app.svgator.com/).
