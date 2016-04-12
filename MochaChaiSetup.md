#Mocha Chai Setup -- for integration testing

Assumes you are using Galvanize Express Generator and that mocha is installed globally

##Steps

1. Create a 'test' directory in the project root
1. Install dependencies:

  ```sh
  $ npm i chai chai-http mocha --save-dev
  ```
1. Add a 'test' script to *package.json*:

  ```json
    "test": "mocha" 
  ```

1. Add a new file called *mocha.opts* to the 'test' directory and add the following flag so hat mocha looks in all the directories with the 'test' directory for tests:

  ```--recursive
  ```
1. Create a new foler call 'integration' within the test directory.