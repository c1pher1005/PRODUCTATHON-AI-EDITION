# Login With the Help of Blockchain

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









# For Running Blockchain Based E-Vault

Submission for the E-Suraksha hackathon at CU

- [Blockchain Based E-Vault](#blockchain-based-e-vault)
  - [Team members](#team-members)
  - [Tech Stack](#tech-stack)
- [How to run](#how-to-run)
  - [Fork and Clone the repo](#fork-and-clone-the-repo)
    - [Run the frontend](#run-the-frontend)
    - [Run the backend](#run-the-backend)
    - [Blockchain](#blockchain)
      - [Run a local arweave node](#run-a-local-arweave-node)
      - [Deploy the smart contract](#deploy-the-smart-contract)
      - [Tests for the contract](#tests-for-the-contract)

## Team members
- Parth Tiwari
- Divyanshu Sah

## Tech Stack

- React
- Vite
- Arweave Blockchain
- Arweave.app web wallet
- arweavekit

# How to run

## Fork and Clone the repo

```bash
git clone https://github.com/<YOUR_USERNAME>/esuraksha-cu.git
```

The project is split into 3 folders

- `app` - React frontend
- `instabase` - Express backend with instabase functions
- `contracts` - Arewave Smart contracts to store document data

### Run the frontend

```bash
cd app
npm install --force
```

```bash
npm run dev
```

### Run the backend

```bash
cd instabase
npm install --force
```

```bash
nodemon index.js
```

### Blockchain

#### Run a local arweave node

```bash
npx arlocal
```

#### Deploy the smart contract

```bash
cd contracts
npm install --force
```

**Smart Contract is in `contracts/contract.js`**

```bash
node deploy.js
```

#### Tests for the contract

```bash
node write.js
```

```bash
node read.js
```

**NOTE: All of these should be run with arlocal running in the background or in a terminal tab**

To make sure the contract deploys you will need an arweave `wallet.json` file which can be created using `ardrive-cli` or downloaded from arweave.app web wallet
