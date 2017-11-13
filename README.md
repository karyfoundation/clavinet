
# Clavinet
Clavinet is a command line argument parser with it's own language rules. It joins the given `process.argv` into a string and then parses it with it's own language grammar.

## Language
Clavinet has these concepts:

- __Commands__ &mdash; Commands start with double dashes as `--some-command-name` and they can have a value after them separated by spaces like: `--say hello`, or `--add [2, 3, 5]`
- __Values__ &mdash; Values are __Literals__ or __Arrays__
- __Array__ &mdash; Array is made of a sequence of __Values__ separated by `,` and inside of square bracket. For example: `[1, 2, 4, hello, [1, 3]]`
- __Literals__ &mdash; Literals are numbers and words in this format: `[a-zA-Z0-9_\./][a-zA-Z0-9_\.\-/]*`

## Building
You need to run `npm install` to install all the dependencies and you must have _TypeScript_ installed on your system. After that you can build the package using

```
npm run build
```

## How to use it?

First install it via

```sh
npm install --save clavinet
```

Then use it as:

```js
const clavinet = require('clavinet')
const args = clavinet.Parse( )
```


<br><br>
<img src="https://user-images.githubusercontent.com/2157285/28680500-c9ca905a-730b-11e7-99bf-2b249d97c17d.png" width="260">