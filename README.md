# Form Builder User Data Store client (Node)

Client for making requests to Form Builder platform user datastore endpoints

## Requirements

Node

## Installation

`npm install @solidgoldpig/fb-user-datastore-client-node`

## Usage

### Loading and initialising

``` javascript
// load client
const FBUserDataStoreClient = require('@solidgoldpig/fb-user-datastore-client-node')

// initialise client
const userDataStoreClient = new FBUserDataStoreClient(serviceSecret, serviceToken, serviceSlug, userDataStoreUrl)
```

### Fetching and storing

``` javascript
// fetch user data
const userData = await userDataStoreClient.getData(userId, userToken)

// store user data
await userDataStoreClient.setData(userId, userToken, userData)
```

