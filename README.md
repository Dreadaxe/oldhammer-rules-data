# Oldhammer Rules — open data

Machine-readable transcription of the **Warhammer Fantasy Battle 3rd edition** rulebook,
maintained by the [Oldhammer Rules Index](https://oldhammer-wfb.lovable.app) and open to any
application that wants to build on top of it.

## Layout

```
content/<book>/<slug>.md   one chapter per file, YAML front matter + markdown
data/index.json            list of every page with its title, category and printed pages
data/glossary.json         glossary terms, aliases, definitions and target pages
```

## Markdown conventions

- `{{p:NN}}` after a heading is a **printed page citation** from the original book.
- `[[slug|label]]` is an internal link to another page of this repository.
- Tables are standard GitHub-flavoured markdown.

## Reading the data

Raw files:

```
https://raw.githubusercontent.com/Dreadaxe/oldhammer-rules-data/main/data/index.json
```

JSON API (no key required, CORS enabled):

```
https://oldhammer-wfb.lovable.app/api/public/v1/pages
https://oldhammer-wfb.lovable.app/api/public/v1/pages/{slug}
https://oldhammer-wfb.lovable.app/api/public/v1/glossary
https://oldhammer-wfb.lovable.app/api/public/v1/search?q=charge
https://oldhammer-wfb.lovable.app/api/public/v1/version
```

## Contributing

Pull requests are welcome. Corrections submitted on the wiki are validated by editors and
opened here as pull requests automatically; changes merged here flow back into the wiki.

The rules text is the property of Games Workshop; this repository exists for preservation
and interoperability, not for commercial use.
