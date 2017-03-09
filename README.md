# Ractive.js Website

## Setup

```sh
# Install the following. Installation procedure may vary by platform.
# - Python 2.7
# - pip
# - virtualenv

# Create a virtualenv and activate it
virtualenv ractivejs.github.io
cd ractivejs.github.io
source ./bin/activate

# Fork this repo and clone your fork.
git clone git@github.com:YOUR_USERNAME/ractivejs.github.io.git src
cd src

# Install dependencies
pip install -r requirements.txt
```

### Development

```sh
# Serve the site
mkdocs serve

# Build the site
mkdocs build

# When done developing, deactivate the virtualenv
deactivate
```

Refer to the [mkdocs site](http://www.mkdocs.org) for more information.

### Style guide

- Add the page title as the first and only first-level header.
- Use the appropriate markdown construct for the text.
- For instance members, prefix with `ractive.`.
- For static members, prefix with `Ractive.`.
- For functions, suffix with `()`.
- Be aware that headings 1, 2 and 3 appear on the sidebar.

## Notes

- Everything is written in vanilla Markdown.
- Everything goes in the `docs` directory.
- Old documentation can be found in the `legacy` directory.
- The nav bar is managed in `mkdocs.yml`.
