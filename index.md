## Post a dish

The Makefile script requires you to `git add src/dish.md`, `git commit -a -m "dish title"` and `git push` the markdown article as it needs to log the author and creation date via git commits to build it, otherwise it won't appear on the site.

## Update (build) the site

Go to the `food` directory and run the command below.

```
make build
```

The first time you will need to apply css changes. You also need to deploy to upload pictures

```
make deploy
```

### Troubleshooting

If `make` doesn't work you'll probably need to install missing programs, such as `markdown`. Installing the latest version is often the best choice, sometimes the installing package with the latest version doesn't have the same name as the program, but it does contain it if the package manager shows it in the list.

To apply additional css changes you'll actually need to remove the blog/style.css file and then deploy again. Alternatively you can run:

```
make clean;
make build;
make deploy;
```

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
