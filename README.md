# Lab 1 - Single Page App Hosting on Azure Storage

This lab will walk you through hosting a front-end JavaScript app with Azure Storage. 
This is a cheap and fast way to host self contained, front end assets like React/Angular/Vue apps.

## Checkout and build the React Single Page App (SPA) locally
1. Open the integrated terminal in Visual Studio Code with `ctrl + tilde`
2. Clone and open the code in this repository with VS Code.

```
cd ~/Downloads
git clone https://github.com/pjmeyer/lab1-spa.git
cd lab1-spa ; code . -r
```

3. Run `npm install` to get the dependencies
4. Run `npm run build` to build locally
5. Run locally with `npm run start`
6. You should see the following:
<img width="718" alt="image" src="https://user-images.githubusercontent.com/820883/46748497-90a1fb80-cc68-11e8-9de3-f60029f7866a.png">


## Deploy the same app to the cloud!

1. Right-click on your `build` folder, and select the option, `Deploy to static website`
<img width="360" alt="deploy-static-retina" src="https://user-images.githubusercontent.com/5591113/46822533-9a972d80-cd40-11e8-88dc-4a09d4c073a4.png">

3. You'll be asked to select a resource ggroup. Choose the "jsineractive[x]" group.

4. A warning will popup that says "The storage container "jsinteractive[x]/$web" contains 15 files. Deploying will delete all of these existing files.  Continue?" Choose **Delete and deploy**

5. When deployment completes, you'll see a notification in the bottom right. Click `Browse to Website`

<img width="463" alt="image" src="https://user-images.githubusercontent.com/820883/46750293-7a963a00-cc6c-11e8-9181-1698e114e7c7.png">


## Make a code change
1. Back in VS Code, open `src/App.js` and make a change. If you're unfamiliar with React, that's ok, find **line 12** and edit the text.
<img width="954" alt="image" src="https://user-images.githubusercontent.com/820883/46750203-4d498c00-cc6c-11e8-9ae2-efa9cb371a44.png">

2. Rebuild with `npm run build`

3. Re-deploy following the same steps in the above section

## Summary
This lab shows you how quickly and easily you can deploy a front-end app to Azure Storage using Visual Studio Code and the Azure Storage extension. These tools allow for rapid iteration and deployment.

## All Done!

