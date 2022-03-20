# Node Typescript Single File Boilerplate

## Motivation

To create scripts using typescript and distribute them as single javascript file (to be executed with node) or binary.

## Usage

Create your code inside `src` folder. The function `main()` inside `index.ts` is the program entry point.

You can then make use of one of the following scripts.

### npm start

Execute your code. Mainly for testing purposes.

### npm run build
Bundle your code into a single `index.js` file inside the `/dist` folder. You can execute with `node index.js` assuming you have node installed.

### npm run compile
Compile your code to a binary named `index` inside the `/dist` folder. By default, the target architecture will be the one compiling the code.

This script inside VSCode (or other editors); instead execute in the terminal directly to avoid injecting unwanted variables to your node process.

To target other architectures, you can edit the `package.json` file and add -t flag to the compile script. Check out pkg documentation https://github.com/vercel/pkg

## Important dependencies

This boilerplate uses two very handy packages:
- https://github.com/vercel/ncc
- https://github.com/vercel/pkg
