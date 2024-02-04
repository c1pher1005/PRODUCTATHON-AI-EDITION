## Idea Description:The legal field, like other industries, has experienced notable technological advancements in recent times. Our company's cutting edge JurisTech platform is leading the way, in these innovations by providing a comprehensive and intelligent Automated Case Management system that meets the requirements of professionals and stakeholders. This system incorporates technologies each playing a distinct role in improving the legal process.

# For Running Landing Page simply load it in VS Code and hit the Live Server button 


  # replit url : https://replit.com/@parthtiwari1005/PRODUCTATHON-AI-EDITION



## Here are the Screenshots of the product and how it will look :
<img width="1440" alt="Screenshot 2024-02-04 at 12 53 49 AM" src="https://github.com/c1pher1005/PRODUCTATHON-AI-EDITION/assets/114827938/9361fdc0-de18-4cb1-9b87-3ee8c83fe762">


  
  ## this is the landing page 


<img width="1440" alt="Screenshot 2024-02-04 at 12 54 04 AM" src="https://github.com/c1pher1005/PRODUCTATHON-AI-EDITION/assets/114827938/698a7aca-5bd4-4b90-8023-4c59b23193cb">



   ### This is the Role Based Login Window which will be using the Ethereum and polygon to perform the login task


<img width="1440" alt="Screenshot 2024-02-04 at 12 54 10 AM" src="https://github.com/c1pher1005/PRODUCTATHON-AI-EDITION/assets/114827938/02de80e9-1ca0-4303-8cf0-a4af9192c6a6">


  ### With the help of the following wallets you can easily log in according to your role 


![WhatsApp Image 2024-02-04 at 01 15 56](https://github.com/c1pher1005/PRODUCTATHON-AI-EDITION/assets/114827938/78d3998e-3bde-44b0-a310-2e0487de62ec)


this is the admin panel for judges where he can manage the cases etc with case summarizer functionality 



![WhatsApp Image 2024-02-04 at 00 56 14 (1)](https://github.com/c1pher1005/PRODUCTATHON-AI-EDITION/assets/114827938/3cc68ee2-6beb-449e-a4b4-4d57767149c1)


### Across the website there will be chatbot support that will be answering all your doubts easily as shown above 



<img width="1440" alt="Screenshot 2024-02-04 at 1 09 12 AM" src="https://github.com/c1pher1005/PRODUCTATHON-AI-EDITION/assets/114827938/2d5f88f7-2a18-4d20-b09e-9667fa1bb865">



### This is the case of Summerizer which is based on LLM powered chatbot , it uses OpenAI Api key, Streamlight, and LangChain




![WhatsApp Image 2024-02-04 at 02 23 02 (1)](https://github.com/c1pher1005/PRODUCTATHON-AI-EDITION/assets/114827938/f4e69adf-e510-47a9-bf82-cbb2a81218de)


### This is the E-vault for legal records which uses the Arweave Blockchain because it can store a large amount of data and its gas fees are also very very low.


 # Now, to install it on the local host follow the below steps 




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
