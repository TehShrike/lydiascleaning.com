## To generate the font subset

Install [pyftsubset](https://fonttools.readthedocs.io/en/latest/subset/):

```sh
pip install fonttools
```

### Generate the subset for the title

Generate `DancingScript.subset.ttf`:

```sh
cd docs
pyftsubset DancingScript.woff --text="Lydia's Cleaning"
```

### Generate the subset for the body

```sh
npx glyphhanger docs/index.html --subset=docs/NotoSansKR-Light.otf --formats=ttf
```