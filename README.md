# openRxiv brand in YAML

## Description

This repository contains the `_brand.yml` and custom `styles.scss` for openRxiv to be used with Quarto documents.

The brand implements the corporate colors, font, and logo for openRxiv.


## Usage

From a folder containing a Quarto document, run in the Terminal:

```bash
quarto use brand openrxiv/brand-openrxiv
```

This copies brand files from the external source into your project’s `_brand/` directory.

It does not copy the `styles.css` or `styles.scss` files. To use a style file in this repo, you can add the following to the yaml header of your Quarto doc:

```yaml
format:
    #[html, revealjs]:
        css: https://cdn.jsdelivr.net/gh/openrxiv/brand-openrxiv@main/[path-to-css-from-root]
```

To convert any path in GitHub to jsDelivr, use this [link](https://www.jsdelivr.com/github).

For more details: [Multiformat branding with _brand.yml](https://quarto.org/docs/authoring/brand.html#sharing-brands-across-projects)