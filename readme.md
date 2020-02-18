# TypeScript
#### Try At Least Once (JavaScript libraries and frameworks) > JavaScript Flavors > TypeScript

Official website: [https://www.typescriptlang.org](https://www.typescriptlang.org/ "https://www.typescriptlang.org")
Github repository: [https://github.com/Microsoft/TypeScript](https://github.com/Microsoft/TypeScript "https://github.com/Microsoft/TypeScript")

------------
When creating TypeScript, Microsoft had the motto “JavaScript that scales.” It is much easier to maintain a large codebase with TypeScript because it simplifies the JavaScript code, it includes tools to increase the effectiveness of developers and has a very powerful type system.

Everything that can be written in JavaScript can also be written in TypeScript.The most important difference between TypeScript and JavaScript is that they are two separate programming languages, though TypeScript is heavily based on JavaScript. TypeScript is a superset of JavaScript, meaning all valid JavaScript code is also valid TypeScript code.

Based on the [Stack Overflow Developer Survey in 2019](https://insights.stackoverflow.com/survey/2019 "Stack Overflow Developer Survey in 2019"), TypeScript is more "loved" as a programming language than JavaScript. The reason is because of adding types to JavaScript which allows developers to catch the errors before running the code.

## How to use TypeScript
The command-line TypeScript compiler can be installed as a Node.js package.

### Installation
- NPM Installation Method

`npm install -g typescript`

- Yarn Installation Method

`yarn global add typescript`

To quickly test that the setup works, you can create a test TypeScript file and then run tsc in the command line and see if a JavaScript file is generated beside the TypeScript file.

### Quick Example
As mentioned above, create **greeter.ts**  file then start to write our greeter function.
```
// greeter.ts file
function greeter(person: string) {
    return "Hello, " + person;
}
let user = "Jeff Bezos";
window.alert(greeter(user));
```

and compile your greeter.ts file in command line:

```
tsc greeter.ts
```
after the compile, you will find **greeter.js** file which has pure JavaScript code.

In this sample, greeter function has been called with a single string parameter. If you change the value of **user** variable to a number and re-compile it, you'll get an error like this:

`greeter.ts - error TS2345: Argument of type 'number' is not assignable to parameter of type 'string'`