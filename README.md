selfpub-example
===============

Example selfpub ebook source. See [selfpub](https://github.com/BjoernSchotte/selfpub) for ebook build scripts.

# standard ebook layout

The layout of a selfpub ebook is standardized to keep things as simple as possible. After you clone this repo (or download the ZIP), you have the following directory structure:

```
de                       → if your ebook is available in German language
 └ 00-title.txt          → title + author of the ebook (pandoc format)
 └ 01-nameyourchapter.md → first chapter in markdown format. Choose whatever filename you wish
en
 └ 00-title.txt          → title + author of the ebook (pandoc format)
 └ 01-nameyourchapter.md → first chapter in markdown format. Choose whatever filename you wish
cover
 └ de-cover.jpg          → cover for German ebook
 └ en-cover.jpg          → cover for English ebook
images                   → contains images you refer from your chapters
epub                     → contains epub specific files
 └ metadata.xml          → dublin core metadata
out                      → directory which contains the generated eBook files, on demand
```

As you see, you can have as many languages for your ebook as you want - "de" and "en" comes by default in the directory structure. The language prefix must also be when you define the cover image.

The file names of the chapters are as you like, prefixing them with numbers as you go.

# contributing

If you want to contribute, please create a feature branch and open a pull request, or open github issues if you want to report bugs.
