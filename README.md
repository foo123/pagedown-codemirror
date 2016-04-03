PageDown CodeMirror
===================

**in progress**

**PageDown CodeMirror** is a port of [PageDown](https://code.google.com/p/pagedown/wiki/PageDown) running with [CodeMirror editor](https://codemirror.net/) instead of a (plain) `textarea`.

Basically:

```html
    <div id="wmd-button-bar"></div>
    <div id="wmd-input"></div>
    <script type="text/javascript">
        var converter = new Markdown.Converter();
        var editor = new Markdown.Editor(converter);
        var cm = CodeMirror(document.getElementById("wmd-input"),{value:"some text",lineNumber:true});
        editor.run(cm);
    </script>
```

The [demo page][1] has been updated accordingly.


  [1]: https://github.com/foo123/pagedown-codemirror/blob/master/demo/browser/demo.html