# Lab 1 - Singe Page App Hosting on Azure Storage

This lab will walk you through hosting a front-end JavaScript app with Azure Storage. 
This is a cheap and fast way to host self contained, front end assets like React/Angular/Vue apps.

## Checkout and build the React Single Page App (SPA)
1. Open the integrated terminal in VS Code with `ctrl + tilde`
2. Clone and open the code in this repository with VS Code.
```
cd ~/Downloads
git clone https://github.com/bowdenk7/lab1-spa.git
cd lab1-spa ; code . -r
```
3. Run `npm install` to get the dependencies
4. Run `npm run build` to build locally
5. Run locally with `npm run start`
6. You should see the following:
<img width="718" alt="image" src="https://user-images.githubusercontent.com/820883/46748497-90a1fb80-cc68-11e8-9de3-f60029f7866a.png">


## Your First Deployment
1. Open the Azure tab on the left side of VS Code

2. Open the storage section

3. Open the demo subscription: `CADDAI Backups` 
<img width="391" alt="image" src="https://user-images.githubusercontent.com/820883/46748625-d3fc6a00-cc68-11e8-98c7-b8febbff43e8.png">

4. Right click the storage account that corresponds to your machine number (ie. jsinteractive<machineNumber>) and choose  `Deploy to static website`. 
  
5. A warning will popup that says "The storage container "jsinteractive4/$web" contains 15 files. Deploying will delete all of these existing files.  Continue?" Choose **Delete and deploy**
  
6. Choose browse and select the `build` folder. This contains the React SPA you just built locally.
<img width="605" alt="image" src="https://user-images.githubusercontent.com/820883/46748737-158d1500-cc69-11e8-84fc-1ad22fdeaeac.png">

7. When deployment completes, you'll see a notification in the bottom right. Click `Browse to Website`
<img width="463" alt="image" src="https://user-images.githubusercontent.com/820883/46750293-7a963a00-cc6c-11e8-9181-1698e114e7c7.png">


## Make a code change
1. Back in VS Code, open `src/App.js` and make a change. If you're unfamiliar with React, that's ok, find **line 12** and edit the text.
<img width="954" alt="image" src="https://user-images.githubusercontent.com/820883/46750203-4d498c00-cc6c-11e8-9ae2-efa9cb371a44.png">

2. Rebuild with `npm run build`

3. Redeploy following the same steps in the above section

## Summary
This lab shows you how quickly and easily you can deploy a front-end app to Azure Storage using VS Code and the Azure Storage extension. These tools allow for rapid iteration and deployment.

## All Done!

