# react-pages

## Deploy the React app on GitHub Pages

### 1. Create a "react-pages" repository
```http
https://github.com/<username>/react-pages
```

### 2. Implementation environment
```sh
$ node -v
v12.18.3
$ npm -v
6.14.6
$ create-react-app --version
4.0.1

# Install "create-react-app"
$ npm install -g create-react-app
```

### 3. make
```sh
$ create-react-app react-pages
$ cd react-pages
$ npm install gh-pages --save-dev
$ nano package.json
//...
"homepage": "http://<username>.github.io/react-pages",
"scripts": {
  //...
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
$ git init
$ git remote add origin git@github.com:<username>/react-pages.git
$ npm run deploy
```


### 4. access
```http
https://<username>.github.io/react-pages/
```

<br>

### Created real thing
[react page](https://scgajge12.github.io/react-pages/)

