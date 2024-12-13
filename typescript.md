## What is TypeScript?

TypeScript is a language that has all the same features and syntax as Javascript and behaves identically at runtime.
However, it adds a static type checker with the caveat that all types are erased at runtime to preserve the behaviour of javascript.
This is so that it is easy to transition between the languages without worrying about anything breaking.

## Javascript Vs TypeScript

Javascript has a number of strange quirks such as:
    - Allowing the referencing of non-existent properties
    - Its equality operator coercing operands
    - Math.min() is greater than Math.max()
    - The expression true + true + true evaluates to 3
    - NaN is not equal to NaN
    - Many, many more

Typescript will produce compiler errors alerting the author in the scenorios where a behaviour is technically legal within javascript but 
may produce unexpected/unwanted behaviour. 

## TypeScript Compiler Options
TypeScript compiler options allow you to configure how the TypeScript code is transformed into JavaScript and ensure stricter type checking for improved code quality. These options, defined in a tsconfig.json file or passed via the tsc command, cover various aspects such as specifying the ECMAScript version for output, module system, and libraries. Additionally, compiler options can be used for strict type checking and module resolution settings. Here are some examples of compiler options and their functionalities:
    - target: chooses what version of javascript to transpile your code to
    - lib : the set of language features you want typescript to compile
    - module: the module system that the outputted js will operate under
    - allowJs: allows javascript files to coexist in a typescript project
    - outDir: defines the path the where the outputted files go
    - strict: used to enable all strict type checking rules such as strictNullChecks, strictFunctionTypes, etc.
    

