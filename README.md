## How to setup a typescript environment

1. **Create a TypeScript project:** You can create a new TypeScript project by running the following commands in your terminal:

    ```bash
    mkdir my-project
    cd my-project
    npm init -y
    ```

    This creates a new directory called my-project, initializes a new Node.js project, and creates a `package.json` file.


2. **Install TypeScript:** You can install TypeScript using the Node Package Manager (NPM) by running the following command in your terminal:

    ```bash
    npm install typescript
    npm install @types/node --save-dev
    ```
    
    This will install typescript in your project `node_modules` folder and also add typescript as a dependency in your `package.json` file.

3. **Configure your code editor:** Configure your code editor to work with TypeScript. This may involve installing additional extensions or plugins, setting up code snippets, and configuring build tasks.

    Create a `tsconfig.json` file using the command below:
    ```bash
    npx tsc --init
    ```


4. **Write TypeScript code:** With your environment set up, you can start writing TypeScript code! You can create a new TypeScript file with the `.ts` extension and start writing TypeScript syntax. For example:
    ```javascript
    function greet(name: string) {
      console.log(`Hello, ${name}!`);
    }

    greet('World');
    ```

5. **Compile TypeScript code:** To run TypeScript code, you'll need to compile it to JavaScript using the TypeScript compiler. You can do this by running the following command in your terminal:
    ```bash
    npx tsc my-file.ts
    ```

    This will compile the `my-file.ts` file to JavaScript and generate a new file called `my-file.js`.


## How to configure typescript compiler

```json
/*tsconfig.json file settings*/
{
  "compilerOptions": {
    "target": "ES6",              /* Set the JavaScript language version for emitted JavaScript and include compatible library declarations. */
    "module": "ES6",              /* Specify what module code is generated. */
    "outDir": "./dist",           /* Specify an output folder for all emitted files. */
    "strict": true,               /* Enable all strict type-checking options. */
    "skipLibCheck": true          /* Skip type checking all .d.ts files. */
  },
  "include": ["src/"]             /* Specify a folder where your typescript files are located and will be compiled from */
}
```
