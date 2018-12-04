# Babel bug example

- `yarn install`
- `yarn test`

Error:

```js
yarn test
yarn run v1.12.3
warning package.json: No license field
$ babel src -d lib
SyntaxError: /Users/hsuting/Desktop/work/test/src/index.js: Decorators are not enabled.
> 1 | @decorator
    | ^
  2 | class Test {
  3 | }
  4 | 
    at File.buildCodeFrameError (/Users/hsuting/Desktop/work/test/node_modules/@babel/core/lib/transformation/file/file.js:261:12)
    at NodePath.buildCodeFrameError (/Users/hsuting/Desktop/work/test/node_modules/@babel/traverse/lib/path/index.js:157:21)
    at verifyUsedFeatures (/Users/hsuting/Desktop/work/test/node_modules/@babel/helper-create-class-features-plugin/lib/features.js:39:16)
    at PluginPass.Class (/Users/hsuting/Desktop/work/test/node_modules/@babel/helper-create-class-features-plugin/lib/index.js:69:42)
    at newFn (/Users/hsuting/Desktop/work/test/node_modules/@babel/traverse/lib/visitors.js:193:21)
    at NodePath._call (/Users/hsuting/Desktop/work/test/node_modules/@babel/traverse/lib/path/context.js:53:20)
    at NodePath.call (/Users/hsuting/Desktop/work/test/node_modules/@babel/traverse/lib/path/context.js:40:17)
    at NodePath.visit (/Users/hsuting/Desktop/work/test/node_modules/@babel/traverse/lib/path/context.js:88:12)
    at TraversalContext.visitQueue (/Users/hsuting/Desktop/work/test/node_modules/@babel/traverse/lib/context.js:118:16)
    at TraversalContext.visitMultiple (/Users/hsuting/Desktop/work/test/node_modules/@babel/traverse/lib/context.js:85:17)
error Command failed with exit code 1.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```
