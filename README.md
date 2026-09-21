# openRxiv brand in YAML

## Usage

The `git submodule add` command copies brand files from a private GitHub repository into your project (using HTTPS credentials) in a new `shared-brand/` directory. To use it, navigate to your project directory and run:

**Terminal**
```bash
git submodule add https://github.com/openrxiv/brand-openrxiv.git shared-brand
```

For a presentation, make sure the YAML header in the Quarto document includes:

```r
format:
  revealjs:
    css: shared-brand/styles.css
    footer: " "
    brand: shared-brand/_brand.yml
```
