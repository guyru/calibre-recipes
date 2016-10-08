# Calibre Recipes

A collection of Calibre news recipes targeting. The collection currently has:

 * `haaretz.recipe` - Recipe for [Haaretz (הארץ)](http://www.haaretz.co.il).
 * `haaretz_images.recipe` - Recipe for [Haaretz (הארץ)](http://www.haaretz.co.il), same as `haaretz.recipe` but also saves the images.
 * `alaxon.recipe` - Recipe for [Alaxon (אלכסון)](http://www.alaxon.co.il/).

# Usage
```
ebook-convert ./alaxon.recipe alaxon-`date +%F`.azw3
```

Now you can copy your the resulting `azw3` file to your Kindle. Note that the resulting file isn't exactly a Kindle Periodical, as the `azw3` format doesn't support it. But Kindle doesn't support RTL for `mobi` files so this is the best solution. 

The recipes for Haaretz require you to additionally pass `--username` and `--password` with your username and password for authentication with the site.
