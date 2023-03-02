# Core JS 101

:warning: **Please note that you mustn't open PRs that contains the answers to [this repo](https://github.com/mikhama/core-js-101)!**

However, PRs with the fixes or proposals are welcomed!

---

## Stack
* JavaScript (ES6)
* Webpack
* Git

---

## Task
The task is to implement functions on different Core JS topics. There are eight modules with different tasks. Each module consists of tasks for specified topic:

1. [Strings](https://github.com/Tatty13/core-js-101/blob/master/src/01-strings-tasks.js)
2. [Numbers](https://github.com/Tatty13/core-js-101/blob/master/src/02-numbers-tasks.js)
3. [Arrays](https://github.com/Tatty13/core-js-101/blob/master/src/03-arrays-tasks.js)
4. [Date](https://github.com/Tatty13/core-js-101/blob/master/src/04-date-tasks.js)
5. [Objects](https://github.com/Tatty13/core-js-101/blob/master/src/05-objects-tasks.js)
6. [Promises](https://github.com/Tatty13/core-js-101/blob/master/src/06-promises-tasks.js)
7. [Conditions and Loops](https://github.com/Tatty13/core-js-101/blob/master/src/07-conditions-n-loops-tasks.js)
8. [Functions and Closures](https://github.com/Tatty13/core-js-101/blob/master/src/08-functions-n-closures-tasks.js)

**Active usage of [documentation](https://developer.mozilla.org/en-US/) is strongly recommended!**

## Prepare and test
1. Install Node.js
2. Fork this repository: https://github.com/mikhama/core-js-101/
3. Clone your newly created repo: `https://github.com/<%your_github_username%>/core-js-101/`
4. Go to folder `core-js-101`
5. To install all dependencies use `npm install`
6. Each task is usually a regular function:
    ```javascript
      /**
       * Returns the result of concatenation of two strings.
      *
      * @param {string} value1
      * @param {string} value2
      * @return {string}
      *
      * @example
      *   'aa', 'bb' => 'aabb'
      *   'aa',''    => 'aa'
      *   '',  'bb'  => 'bb'
      */
      function concatenateStrings(value1, value2) {
        throw new Error('Not implemented');
      }
    ```
    Read the task description in the comment above the function. Try to understand the idea. You can see the tests prepared if you don't understand it.
7. Write your code in `src/*.js`.

    Remove the throwing error line from function body:
    ```javascript
        throw new Error('Not implemented'); 
    ```
    Implement the function by any way and verify your solution by running tests until the failed test become passed (green).
8. Run `npm test` in command line. If everything is OK you can try to resolve the next task.
9. You will see the number of passing and pending tests: `101` of passing tests is equal to `100` in score.

## Notes
* We recommend you to use nodejs of version 14 or lower. If you using any of features that does not supported by node `v14`, score won't be submitted.
* Please be sure that each of your test in limit of 30sec.
* You will get 0 (zero) if you have any eslint's errors or warnings.

## FAQ
**Question:** I use Windows machine and have received a lot of errors like "Expected linebreaks to be 'LF' but found 'CRLF'". How to handle it?

**Answer**:
- First, you need to install Gitbash properly: you need to choose option "Checkout as-is, commit as-is" in section "Configuring the line ending conversions". It'll let you download repos with line endings set "as-is" as well as commit. In other words, not to change them at all, because by default it converts them.
- Second, install `editorconfig` plugin to your editor. For VS Code you can find it here:
https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig

  I'll let you apply some rules when you saving your files in the repo. This plugin will use config-file `.editorconfig` that you can see in the root folder. It lets you save the file with needed line endings, trim whitespaces, etc.
- Finally, you need to apply linter's autofix feature in order to fix all linebreaks that was already changed to "CLRF":
```
$ npm run lint -- --fix
``` 

___
The task based on https://github.com/rolling-scopes-school/js-assignments.
