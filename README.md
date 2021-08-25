# vscode-snippets

A repo of useful VS Code snippets

## To add snippets in VS Code

This page from the VS Code docs explains it better than I could:
https://code.visualstudio.com/docs/editor/userdefinedsnippets#_create-your-own-snippets

Once you've created your snippet file(s), just copy and paste any of the snippets in this repo that you find useful, and you're good to go!

## Calling Snippets

Snippets that return a function do NOT return a named function, but instead return the body of an anonymous function. In other words you'll need to call these snippets like this:

```
const variableName = {{snippet}}
```

Where `{{snippet}}` is the spot you call the shortcut for the snippet you need.

Example:

```
const randomNum = {{random}}

would turn into:

const randomNum = (maxVal = 1) => {
  return Math.floor(Math.random() * maxVal);
};
```

## ES6 Support

All snippets are written with ES6 where possible.

## TypeScript

All TypeScript snippets will be typed where appropriate.

## Default Parameters

Function snippets will have default parameters where deemed appropriate. If you prefer to not have default parameters, or want different ones, just edit the snippets as you see fit.
