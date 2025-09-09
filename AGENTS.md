# Repository Overview

This AGENTS guide describes the purpose of each folder and notable file in this repository.

## Root Files
- **README.md** – Project description and general usage notes.
- **license.txt** – License information for the project.
- **package.json** – Node dependencies and npm scripts.
- **package-lock.json** – Locked versions of npm dependencies.
- **next.config.js** – Next.js framework configuration.
- **jsconfig.json** – JavaScript configuration for path aliases.
- **tailwind.config.js** – Tailwind CSS configuration.
- **postcss.config.js** – PostCSS setup used by Tailwind.
- **vercel.json** – Deployment settings for Vercel.

## Directories
### `components/`
Reusable React components for the UI.
- **Layout.js** – Wraps pages with the site header and footer.
- **Top.js** – Header navigation and theme toggle.
- **Bottom.js** – Footer with dataset links and project credits.
- **jsonlint.js** – Core JSON linting editor component.
- **JSONStringifier.js** – Converts JSON to an escaped string form.
- **xmltojson.js** – Converts XML input to JSON and uses the JSON lint component.

### `contexts/`
React context definitions.
- **ValidContext.js** – Holds the validation state for JSON parsing.

### `hooks/`
Custom React hooks.
- **useExtensionCheck.js** – Checks for the presence of the companion browser extension.

### `markdown/`
Markdown content rendered into site pages.
- **benefits-of-using-a-json-beautifier.md** – Article on the advantages of a JSON beautifier.
- **common-mistakes-in-json-and-how-to-avoid-them.md** – Article covering frequent JSON errors.
- **how-to-open-json-file.md** – Guide on opening JSON files.
- **json-parse.md** – Explanation of JSON.parse usage.
- **json-stringify-guide.md** – Guide to JSON.stringify.
- **mastering-json-format.md** – Overview of JSON formatting best practices.
- **mastering-json-in-javascript.md** – Deep dive into JSON in JavaScript.
- **privacy.md** – Privacy policy information.
- **datasets/** – Markdown descriptions of sample datasets.
  - **emoticons.md** – Details about the emoticons dataset.
  - **programming-languages.md** – Details about the programming languages dataset.
  - **us-states-with-detail.md** – Details about the US states dataset.

### `pages/`
Next.js page components.
- **_app.js** – Custom app wrapper; sets up layout.
- **index.js** – Home page providing the JSONLint editor.
- **json-stringify.js** – Tool page for converting JSON to strings.
- **xml-to-json.js** – Tool page for converting XML to JSON.
- **json-formatter.js** – Marketing page for the JSON Formatter Chrome extension.
- **[...slug]/index.js** – Dynamic renderer for articles and dataset pages based on Markdown files.

### `public/`
Static assets served as-is.
- **browserconfig.xml** – Browser configuration metadata.
- **robots.txt** – Robots exclusion rules.
- **favicon.ico** and icons – Site favicons.
- **datasets/** – JSON dataset files: `emoticons.json`, `programming-languages.json`, `sample.json`, and `us-states-with-detail.json`.
- **fonts/** – MonoLisa font files used for code styling.
- **images/** – Logos, screenshots, and other images used across the site.

### `styles/`
Styling resources.
- **globals.css** – Tailwind-based global styles.

