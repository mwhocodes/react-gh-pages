# react-gh-pages
## This project is testing the deployment to git hub pages

1. **Create an project**
```bash
$ npm create-react-app react-gh-pages
```

2. **Install the `gh-pages` packages as "dev-dependency" of the app**
```bash
$ npm install gh-pages --save-dev
```

3. **Add some properties to `package.json` file of the app**
```json
"homepage": "http://gitname.github.io/react-gh-pages"
```

```json
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
```

4. **Create a git repository in the app's folder**
```bash
$ git init
```

5. **Add the GitHub repository as a "remote" in your local git repository**
```bash
$ git remote add origin https://github.com/gitname/react-gh-pages.git
$ git add .
$ git commit -m "initial commit and publish it to GitHub Pages"
$ git push origin master
```

6. **Deploy the app to GitHub Pages**
```bash
$ npm run deploy
```

7. **Update the changed app**
```bash
$ git add .
$ git commit -m "updates and republish it to GitHub Pages"
$ git push
$ npm run deploy
```
### See the demo: [To-do list project](https://mwhocodes.github.io/react-gh-pages/)









