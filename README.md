# reddit-react-redux-mobile-viewer

not sure how to deploy a react webpack app to vercel...

Not sure the build directory - Vercel says "no directory named public"

# 🚀 Minimalistic React + Redux Mobile Reddit Viewer 🚀

https://github.com/coding-to-music/reddit-react-redux-mobile-viewer

https://reddit-react-redux-mobile-viewer.vercel.app

https://illfixit.github.io/reddit-react-redux-mobile-viewer

From / By https://github.com/illfixit/kind-stranger

https://coding-to-music.github.io/kind-stranger/

## Environment variables:

```java
process.env.NODE_ENV !== 'production'
```

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/reddit-react-redux-mobile-viewer.git
git push -u origin main
```


![screenshot](https://i.redd.it/9go05rx77bx61.jpg)


# Kind Stranger (React Edition)
Minimalistic Mobile Reddit Viewer written in React and Redux

## Demo
You can visit https://illfixit.github.io/kind-stranger to start using it.

## Reviews

```
"Nice app! Thanks for sharing."
```

```
"Sweet project btw!"
```

```
"This is very smooth and fast. Nicely done"
```

```
"Well ya did really good!"
```

### Features
No Google Analytics. No Logins. No Tokens. I don't need your data.

## Adding the GitHub Pages dependency package
Next, we’ll install the gh-pages package in our project. The package allows us to publish build files into a gh-pages branch on GitHub, where they can then be hosted.

Install gh-pages as a dev dependency via npm:

```
npm install gh-pages --save-dev
```
## Adding the deploy scripts
Now, let’s configure the package.json file so that we can point our GitHub repository to the location where our React app will be deployed.

We’ll also need to add predeploy and deploy scripts to the package.json file. The predeploy script is used to bundle the React application; the deploy script deploys the bundled file.

In the package.json file, add a homepage property that follows this structure: http://{github-username}.github.io/{repo-name}

Now, let’s add the scripts.

In the package.json file, scroll down to the scripts property and add the following commands:

```
"predeploy" : "npm run build",
"deploy" : "gh-pages -d build",
```
