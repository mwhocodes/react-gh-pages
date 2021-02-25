# react-gh-pages
## This project is testing the deployment to git hub pages

1. **Create an project**
```bash
$ npm create-react-app react-gh-pages
```

1. **Install the `gh-pages` packages as "dev-dependency" of the app**
```bash
$ npm install gh-pages --save-dev
```

1. **Add some properties to `package.json` file of the app**
```json
"homepage": "http://gitname.github.io/react-gh-pages"
```

```json
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
```

1. **Create a git repository in the app's folder**
```bash
$ git init
```

1. **Add the GitHub repository as a "remote" in your local git repository**
```bash
$ git remote add origin https://github.com/gitname/react-gh-pages.git
```

1. **Deploy the app to GitHub Pages**
```bash
$ npm run deploy
```

1. **Update the changed app**
```bash
$ git add .
$ git commit -m "updates and publish it to GitHub Pages"
$ git push origin master
$ npm run deploy
```
### See the demo: [To-do list project](https://mwhocodes.github.io/react-gh-pages/)









