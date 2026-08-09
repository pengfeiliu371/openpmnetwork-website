# Open PM Network website

Public project website for [Open PM Network](https://www.openpmnetwork.org), an
open, research-first particulate matter sensing platform.

This repository contains only the static public website. Sensor firmware,
server code, hardware documentation, and research notes live in the
[`pm-sensor-node`](https://github.com/pengfeiliu371/pm-sensor-node) repository.

## Architecture

- `www.openpmnetwork.org` â€” this static GitHub Pages website
- `pm.openpmnetwork.org` â€” the separately deployed sensor portal and ingestion API

The public website intentionally contains no device tokens, pairing codes,
private coordinates, Wi-Fi configuration, server secrets, or raw research
databases.

## Local preview

The site uses plain HTML, CSS, and JavaScript. From the repository directory:

```shell
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Publishing

GitHub Pages should publish from the repository root on the `main` branch. The
custom domain will be configured as `www.openpmnetwork.org` after the first
successful Pages deployment.

## License

Website source code is available under the MIT License. Public sensor data is
not included in this repository and will have separate, deployment-specific
publication consent and licensing.

