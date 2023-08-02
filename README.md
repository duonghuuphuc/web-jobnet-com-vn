# Website of JobNet.com.vn


## 1/ Introduction
This private repository contains HTML files and resources of `jobnet.com.vn`


## 2/ Auto Deploy to Firebase
This repository includes **2** YML files to automatically executed to synchronizing files from this repository to the Firebase Hosting, as follows:
- `.github/workflows/firebase-hosting-merge.yml`
- `.github/workflows/firebase-hosting-pull-request.yml`


## 3/ Firebase Hosting INFO
- Project Display Name: `WWW-JobNet`
- Project ID: `jobnet-com-vn-20230801`
- Project Number: `177068726205`


## 4/ Firebase Sites
The `jobnet-com-vn-20230801` Firebase project contains **2** sites: `jobnet-com-vn-20230801` (default), `mta-sts-jobnet-com-vn`.

The configurations of `jobnet-com-vn-20230801` are as follows:
- `Domain`: `jobnet.com.vn`
- `SITE_ID` (aka. `RESOURCE_IDENTIFIER`): `jobnet-com-vn-20230801`
- `TARGET_NAME` (alias name): `www`
- Directory: `~/public/`

The configurations of `mta-sts-jobnet-com-vn` are as follows:
- `Domain`: `mta-sts.jobnet.com.vn`
- `SITE_ID` (aka. `RESOURCE_IDENTIFIER`): `mta-sts-jobnet-com-vn`
- `TARGET_NAME` (alias name): `mta-sts`
- Directory: `~/mta-sts/dist/`


## 5/ Reconfigure the Project
This step is mandatory if you created and initialized the project with a single site at the beginning, and now you want to add other sites to this project to share the same Firebase resources, while also having their own unique domains or content. In particular, you need to perform the following steps:

- Update the `TARGET_NAME` (alias name) of the *default* site with this Firebase CLI command -- `firebase target:apply hosting TARGET_NAME SITE_ID`
- `TARGET_NAME` is an alias name defined by you such as `www`, `web`, `mta-sts`
- `SITE_ID` is the string before the `.web.app` and `.firebaseapp.com` domains
- Example 1: `firebase target:apply hosting www jobnet-com-vn-20230801` to alter the *default* site
- Example 2: `firebase target:apply hosting mta-sts mta-sts-jobnet-com-vn` to alter the *mta-sts-jobnet-com-vn* site
- The above examples will alter the `.firebaserc` file.
- And then, update the `firebase.json` file. The new `firebase.json` is as presented in this repository, you should note that the `hosting` entity is now an array containing sites differentiated by `target` keys (aka. `TARGET_NAME`).


## Useful Links:
- https://firebase.google.com/docs/hosting/quickstart
- https://firebase.google.com/docs/hosting/multisites
- https://firebase.google.com/docs/cli
- https://firebase.google.com/docs/hosting/github-integration
- https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
