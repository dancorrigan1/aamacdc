# AAMA-CDC

A responsive, static website for AAMA Community Development Corporation. No application server or package installation is required.

## Preview

```sh
python3 -m http.server 4173 --bind 127.0.0.1
```

Open http://localhost:4173.

## Editing

- `scripts/build.py`: page content, shared navigation, footer, and legacy redirects.
- `assets/site.css`: responsive layout, typography, and light/dark color tokens.
- `assets/site.js`: accessible mobile navigation.
- `scripts/image-dimensions.json`: original image dimensions, used to reserve layout space.
- `scripts/original-links.txt`: original external resource destinations.

After editing content, regenerate the checked-in HTML:

```sh
python3 scripts/build.py
```

Deploy the generated root HTML files with `assets/`, `images/`, and `TAC/images/`. Include `b768.wmv`, `cleaner256modif.wmv`, and `magnolia.wmv` to support archival video downloads. The `backup/`, `bak/`, `tmp/`, and `nclrphoenix/` HTML files are legacy redirects; include them if those historical URLs were previously public. Do not publish repository archives, `.bak` files, `webstats/`, or development scripts.

## Design and content

The redesign follows the design-taste-frontend skill: design variance 5, motion 3, density 4. It uses native HTML/CSS, self-hosted Manrope, the original blue identity and logo, one 4px corner system, and system-selected light/dark themes. Hover motion respects reduced-motion preferences. Navigation and page content remain usable without JavaScript.

Original photographs are retained. They are low-resolution archival assets; higher-resolution source photographs can replace them later without changing the layout.

Peter Clementi is the sole listed member and contact. His email, the organization’s phone, fax, and address are retained from the original contact page. Former profile and board URLs redirect to the updated staff page, including copies in the old public backup directories.

Project and news pages identify historical information instead of treating old construction plans, events, or financial figures as current. Original page filenames and primary navigation labels are preserved, with the requested board section removed. Original videos are offered as downloads instead of obsolete Internet Explorer embeds.
