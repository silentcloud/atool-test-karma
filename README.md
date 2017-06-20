# atool-test-karma

## Built-in

- [mocha](http://mochajs.org/)
- [chai](http://chaijs.com/api)
- [sinon](http://sinonjs.org/)

## Usage

> Add -test.js suffix with your test files

```
"srcipts": {
  "test": "atool-test-karma"
}
```

with options:

```
atool-test-karma --port 9888 --assert shouldjs --browsers Chrome
```

##  Options

- `--port`: server port, default is 9876;
- `--assert`: run tests with custom assert library <expectjs、shouldjs、chaijs(default)>
- support [karma args](http://karma-runner.github.io/1.0/config/configuration-file.html)

## Browsers & Assert Libs

### Browsers:
>  atool-test-karma --browsers Chrome,Firefox

- Chrome: `npm install karma-chrome-launcher --save-dev`
- Firefox: `npm install karma-firefox-launcher --save-dev`
- IE: `npm install karma-ie-launcher --save-dev`
- Safari: `npm install karma-safari-launcher --save-dev`

### Assert Libs:
>  atool-test-karma --assert expectjs

- expectjs: `npm install karma-sinon-expect --save-dev`
- shouldjs: `npm install karma-should-sinon karma-should karma-sinon --save-dev`
