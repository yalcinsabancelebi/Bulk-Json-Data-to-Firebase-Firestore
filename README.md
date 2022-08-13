## JSON to Firestore
This library allows you to batch and quickly upload your json files to firestore instead of writing them one by one.

#### Features
- A protocol which partitions successfully processed and which failed
- Automatic identification, whether a document should have a supplied name or a randomly generated name

#### Usage
After cloning the repository to your local computer,First of all download [node.js](https://nodejs.org/en/download/ "Node.Js") and then go to compiler run `npm install` and `npm install firebase`. Make sure node_modules is included in your source file.
Go to your Google Firebase account and select your project, if you don't have any projects go to https://firebase.google.com/ create an account and create a project. Name your project and continue.


> Step 1 - go to firebase UI and settings -> project settings
<img src="https://user-images.githubusercontent.com/75809015/184480807-b5b94381-73dd-4c89-90b0-cb3cc0f6cb9d.PNG" width="300">

> Step 2 - service account -> firebase admin sdk -> generate new private key. 
<img src="https://user-images.githubusercontent.com/75809015/184481187-a0251c20-f54f-4b48-b858-5ef6dca293b7.PNG" width="300">

> Step 3 - click on generate key and it will be download
<img src="https://user-images.githubusercontent.com/75809015/184482248-549525ca-8234-4d0d-8f57-bc087848f853.PNG" width="300">

> Step 4 - collect in the same place this all files and rename downloaded json file to 'key.json'. its must be like in this picture
<img src="https://user-images.githubusercontent.com/75809015/184480472-0e719a79-ed5e-47eb-b8bf-41a87a0f1109.PNG" width="300">

> Step 5 - go to general -> click web application
<img src="https://user-images.githubusercontent.com/75809015/184492676-740fed97-05a0-4a9f-9d93-0aee97c5990b.PNG" width="300">

> Step 6 - give the web project a name then and the parts marked in red are important. Copy these three lines and paste them in the appropriate places within the project. Press continue to console.
<img src="https://user-images.githubusercontent.com/75809015/184492689-37914a46-5b1e-473d-a216-5c893916f1ca.PNG" width="300">

Paste the copied sections into the matching sections below. this code block already exists [here](http://localhost/](https://github.com/yalcinsabancelebi/Bulk-Json-Data-to-Firebase-Firestore/blob/92a69424d915d95f1dcad05dd1fe394544023715/Bulk%20Json%20Data%20to%20Firebase%20Firestore/bulk-json-to-firebase.js#L9)) within the project.

```
firebase.initializeApp({
  apiKey: "<YOUR APIKEY>",
  authDomain: "https://<YOUR PROJECTID>-project.firebaseio.com",
  projectId: "<YOUR PROJECTID>"
});
```
