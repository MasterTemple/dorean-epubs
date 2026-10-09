# The Dorean books

Books on the free gospel and the free Word, as [biblix](https://github.com/MasterTemple/biblix)
packages: each folder is a package (`kind = "book"`, an EPUB), and the repository's root is
the Dorean Collection, which brings them all in. All are CC0-1.0.

Each release is published as an archive in this repository's
[releases](https://github.com/MasterTemple/dorean-epubs/releases), listed in the registry's
catalog (the `index` release's `catalog.toml`):

```sh
bx catalog add https://github.com/MasterTemple/dorean-epubs/releases/download/index/catalog.toml --name dorean
bx add dorean:dorean-collection        # every book
bx add dorean:the-dorean-principle     # or one
```

In Obsidian (Topos Bible): *Settings → Registries → Add a registry*, with that URL.

Releasing a book: `cd <its folder> && bx release` (tags `<folder>/v<version>`), then
`bx publish <its folder> --to github:MasterTemple/dorean-epubs`.
