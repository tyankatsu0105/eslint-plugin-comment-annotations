# ESLint plugin comment annotations

🚧WIP🚧

## Feature (still under development)

```bash
$ npm install @tyankatsu/eslint-plugin-comment-annotations
```


```js
// .eslintrc.js

module.exports = {
  plugins: ["@tyankatsu0105/comment-annotations"],
  rules: {
    "@tyankatsu0105/comment-annotations": ["error", {
      'todo': '@todo',
      'fixme': '@fixme',
    }]
  }
};
```

```js
// @Todo <- invalid
const hoge = 'fuga';

// @todo <- valid
const hoge = 'fuga';



// You can also select "fix" option
// @Todo 
const hoge = 'fuga';

// After eslint --fix

// @todo
const hoge = 'fuga';
```

## Inspired by

[eslint-plugin-comment-annotations](https://github.com/102/eslint-plugin-comment-annotations)

## License

MIT