# Setup

Install Sphinx: http://sphinx-doc.org/latest/install.html#mac-os-x-install-sphinx-using-macports

Install the Sphinx Theme: https://github.com/snide/sphinx_rtd_theme

# Build the docs

1. Run `make html`
2. Open the results at _build/html/index.html

# Pushing to the public instance

When you commit changes and push them, a git hook will automatically build and publish the new version of the site via Netlify.

The site is reachable at https://techtabor.miklosdanka.com at the time of writing (2018-09-24).
