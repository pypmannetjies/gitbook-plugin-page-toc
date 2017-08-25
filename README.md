# gitbook-plugin-wiki-toc

Adds a Wikipedia style Table of Contents (TOC) to every page in your GitBook, with anchors link to headings inside the page as well.

Wikipedia style means that the TOC is inserted above the first level 2 heading. That is, it will come after the body of your introduction. 

Only heading levels 2 - 4 are added, or in markdown:

```
# Test

Here you give a brief introduction about the topics on this page. The TOC will be inserted after this paragraph.

## Level 2
### Level 3
#### Level 4
##### Level 5 (not included)
## More Level 2
## More Level 2
## Wow!
```

Will result in a layout like this:

![](https://raw.githubusercontent.com/pypmannetjies/gitbook-plugin-wiki-toc/master/doc/screenshot.png)

This is a fork of [page-toc](https://github.com/aleung/gitbook-plugin-page-toc).

## Install

Add the plugin to your `book.json`:

``` json
    {
      "plugins": [ "wiki-toc" ],
    }
```

## Configuration

Unlike page-toc, there are currently no configuration parameters available for wiki-toc.

## CSS Customization

The TOC elements have class attribute `.page-toc`. You can override the styles in `styles/website.css`.
