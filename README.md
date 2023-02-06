How to get this done?

https://www.geeksforgeeks.org/how-to-deploy-your-react-websites-on-github/

1. create a React application with following command on cmd:
   $ create-react-app my-app

2. my-app folder is created in C drive. Now enter your new application using VS code. Write your code.

3. You will see your application is running on a local development server http://localhost:3000. Run the following command using VS terminal.
   $ npm start

4. Create a repo on Github : my-app

5. Install the gh-pages package as a “dev-dependency” of the app by runing the following command using VS terminal.

   $ npm install --save gh-pages

6)Add some properties to the app’s package.json file.

    "homepage": "https://yadvirkaur.github.io/my-app",

In the existing scripts property, add a predeploy property and a deploy property:

    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",

7. In this step create a git repository in the app’s folder and add the GitHub repository as a “remote” in your local git repository.

   $ git init
   $ git add .
   $ git commit -m "first commit"
   $ git branch -M main
   $ git remote add origin https://github.com/yadvirkaur/my-app.git
   $ git push -u origin main

8. Now here is the magic. Follow the command below and generate a production build of your app, to deploy your code on GitHub pages.

   $ npm run deploy

That’s it. Your React application is published on GitHub pages and if you want to verify it just go to the settings tab of your application in your Github repository and scroll down and click on pages and you will see:

    Your site is live at https://yadvirkaur.github.io/tenziesgame/




    AND ITS DONE!!!!!!!!!!!!!!!!!!!!!

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
