# Code plugin for GitBook

Code blocks are cool but can be cooler. This plugin adds lines numbers for multi-line blocks and a copy button to easily copy the content of your block.

This repository forked from [https://github.com/davidmogar/gitbook-plugin-code](https://github.com/davidmogar/gitbook-plugin-code), removed unnecessary console.log, and fixed the problem of span tags spanning lines.

Go to https://lilu.org.cn/library/ and experience it!

## Cool, can I see it working?

The next image shows a single line code block:

![single line](https://github.com/davidmogar/gitbook-plugin-code/blob/resources/images/single.png?raw=true)

When displaying code with multiple lines, line numbers will be added:

![multi line](https://github.com/davidmogar/gitbook-plugin-code/blob/resources/images/multi.png?raw=true)

When displaying code with newline comments, like the following:

```javascript
/**
 * @author sunchaser admin@lilu.org.cn
 * @since 2022/6/22
 */
module.exports = {
  website: {
    assets: './assets',
    js: [
      'sunchaser-code.js'
    ],
    css: [
      'sunchaser-code.css'
    ]
  }
};
```

## How can I use this plugin?

You only have to edit your book.json and modify it adding something like this:

```json
"plugins" : [ "sunchaser-code" ],
```

This will set up everything for you. If you want to get rid of the copy buttons use add this section too:

```json
"pluginsConfig": {
  "sunchaser-code": {
    "copyButtons": false
  }
}
```
