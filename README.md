# openRxiv brand in YAML

## Usage

The `quarto use brand` command copies brand files from an external source into your project's `_brand/` directory. To use it, navigate to your project directory and run:

**Terminal**
```bash
quarto use brand <source>
```

The source can be a local directory, a GitHub repository, or a URL to a zip archive:

**Terminal**
```bash
quarto use brand https://github.com/openrxiv/brand-openrxiv
```

When you run the command, Quarto walks you through the following steps:

1. If the source is remote, Quarto asks you to confirm that you trust the source.
1. If your project doesn't have a _brand/ directory, Quarto asks to create one.
1. For each file that already exists in your _brand/ directory, Quarto asks whether to overwrite it.
1. Quarto copies all files from the source to your _brand/ directory.
1. If there are files in your `_brand/` directory that don't exist in the source, Quarto asks whether to remove them.


The result is that your `_brand/` directory will match the source exactly, making it easy to stay in sync with a shared brand as it evolves.

Source: [quarto documentation — Sharing brands across projects](https://quarto.org/docs/authoring/brand.html)