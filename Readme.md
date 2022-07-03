# SHELL SCRIPT AND COMMANDS RUN WITH NODEJS

***

- [Ravindu Manoj](https://github.com/ravindu01manoj/)

***

## Installation 
```sh
npm i @ravindu01manoj/bash-js
## or
yarn add @ravindu01manoj/bash-js
```

***

## Example
```ts
const bash = require("@ravindu01manoj/bash-js")

async function run() {

//for single command
const out = await bash.command("ls")
console.log(out)

//for script
const script = `
mkdir a
cd a
touch hello.txt
ls
cd ..
`
const output = await bash.script(script)
console.log(output)
}
run()

```

***
