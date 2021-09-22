## Update (build) the site

Go to the `based.cooking` directory and run (on linux):

```
make build
```

The first time you will need to apply css changes

```
make deploy
```

## Publish a dish

The Makefile script requires you to actually `git commit` and `git push` the `.md` article as it needs to log the author and creation date to build it.

## Tables

Ingridients and their nutrition facts table can be converted to markdown with [https://tabletomarkdown.com/convert-spreadsheet-to-markdown/](https://tabletomarkdown.com/convert-spreadsheet-to-markdown/)

## Tag

Add tags at the end of your recipe with:

```
;tags: tag1 tag2 tag3
```

The tag line should be a single line, at the end of the markdown file, preceded
by a blank line.

## Images

Images are stored in `data/pix`.

## About the site

The front page is just a list of recipes automatically generated
from the content of `src`.

### License

Forked from [https://github.com/LukeSmithxyz/based.cooking](https://github.com/LukeSmithxyz/based.cooking)

This website and all its content is in the public domain.
