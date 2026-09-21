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

After cloning a repo that contains the brand files in this way, you'll see that an empty folder called `shared-brand` is created. You will need to run the following in the terminal to laod them:

```bash
git submodule init
git submodule update
```

See [Git Tools — Submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules) for details.