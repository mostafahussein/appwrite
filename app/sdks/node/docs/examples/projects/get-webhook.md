const sdk = require('node-appwrite');

// Init SDK
let client = new Projects.Client();

let projects = new sdk.Projects(client);

client
    .setProject('')
    .setKey('')
;

let promise = projects.getWebhook('[PROJECT_ID]', '[WEBHOOK_ID]');

promise.then(function (response) {
    console.log(response);
}, function (error) {
    console.log(error);
});