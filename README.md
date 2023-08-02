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
This step is mandatory if you created and initialized the project with a single site at the beginning, and now you want to add other sites to this project to share the same Firebase resources, while also having their own unique domains or content.


## Useful Links:
- https://firebase.google.com/docs/hosting/quickstart
- https://firebase.google.com/docs/cli
- https://firebase.google.com/docs/hosting/github-integration
- https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
