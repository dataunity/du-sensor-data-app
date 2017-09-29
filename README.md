# du-sensor-data-app
This is a [Firebase](https://firebase.google.com) app to post data to
a Data Unity server.

## Seting up
Install the [Firebase command line tool](https://firebase.google.com/docs/cli/):

```
npm install -g firebase-tools
firebase login
```

## Connecting the app to Data Unity
Set up a project for the Firebase app using the [Firebase console](https://console.firebase.google.com).

The Firebase app must be registered with Data Unity by putting your Firebase project id in the UWESENSE_FIREBASE_PROJECT_ID environment variable on the Data Unity server (e.g. put it in the docker-compose.yml file under the web service).

The url in the Firebase app must be changed to point to the instance of Data Unity you're using (search for 'baseUrl' in the index.html file).

## Running the application locally
```firebase --project YOUR_FIREBASE_PROJECT_ID serve```
