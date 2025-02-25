Simple Programs in TypeScript

To run TypeScript programs from the terminal its easy

First install node.js and npm

to verify that node and npm has been installed run theses commands in the command line

the current development environment is WSL2 which is a linux subsystem built into Windows 11. The flavor of Linux is Ubuntu.

    node -v

    npm -v 

Then install typescript globally using npm

    npm install -g typescript

if you run into problems regarding permissions run in sudo

    sudo npm install -g typescript

Then create a new file with the TypeScript extension

    test.ts

Lets make a simple hello world program.

It's a simple program that just needs to have a few parts the first part is creating the variable which is a string that has the text inside the string.

TypeScript is strictly typed as in unlike JavaScript we could write this as 

    var message = "Hello, World"

but instead with TypeScript we have to use the correct syntax for string so it would be written like this

    let message: string = "Hello, World!";

now its as simple as just using the built in console.log command which is 

    console.log(message);

so the full program would be this

    let message: string = "Hello, World!";
    console.log(message);

Now we just have to run the compiler which is the program that compiles TypeScript into JavaScript.

It's really simple just run the compiler tsc

    tsc test.ts

Once the compiler has finished running the output file unless specified will be test.js

now just run the JavaScript file with node

    node test.js
