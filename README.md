# vscode-snippets

A repo of useful VS Code snippets

## To add snippets in VS Code

This page from the VS Code docs explains it better than I could:
https://code.visualstudio.com/docs/editor/userdefinedsnippets#_create-your-own-snippets

Once you've created your snippet file(s), just copy and paste any of the snippets in this repo that you find useful, and you're good to go!

## Other Info

All snippets are written with ES6 where possible.

Snippets that return a function do NOT return a named function. In other words you'll need to call these snippets like this:

```
const variableName = {{snippet}}
```

Where `{{snippet}}` is the spot you call the snippet you need.

Example:
`example.js`

```
const randomNum = {{random}}

would turn into:

const random = (maxVal = 1) => {
  return Math.floor(Math.random() * maxVal);
};
```
