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

It does not copy the `styles.css` or `styles.scss` files. Those need to be manually added to the project folder. [PENDING REVIEW FOR OPTIONS]

For more details: [Multiformat branding with _brand.yml](https://quarto.org/docs/authoring/brand.html#sharing-brands-across-projects)