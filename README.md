React Native 0.57 TypeScript Sample
==========

RN v0.57 Supports TypeScript! This is sample project.

Getting Started
----------

### Setup

```bash
$ git clone git@github.com:Nkzn/ReactNative057Sample.git
$ cd ReactNative057Sample
$ npm install
or
$ yarn
```

### Run App

```bash
# if you don't have cli: npm install -g react-native-cli
$ react-native run-ios
or
$ react-native run-android
```

### TypeCheck

```bash
$ npm run tsc
```

How to create this project
----------

1. `react-native init RN057Sample --version 0.57.0-rc.3` 696d0535
2. rename `App.js` => `App.tsx` and few rewrites. 22ebea7a
    * This is works!
3. Add `@types` modules & TypeScript Compiler 1464655d
4. Setup tsconfig.json for React Native (as below) 2d3922b9
5. That's all! :beer:

```json
{
  "compilerOptions": {
    // from https://blogs.msdn.microsoft.com/typescript/2018/08/27/typescript-and-babel-7/
    "target": "esnext",
    "moduleResolution": "node",
    "allowJs": true,
    "noEmit": true,
    "strict": true,
    "isolatedModules": true,
    "esModuleInterop": true,
    // additional
    "allowSyntheticDefaultImports": true,
    "jsx": "react",
    "lib": ["esnext"]
  },
  "include": [
    "src"
  ]
}
```