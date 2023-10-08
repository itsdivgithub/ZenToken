# Getting Started with ZenToken- Magic SDK

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

Project Description
The objective was to develop an NFT that requires continuous user engagement. The inspiration for this project stems from the concept of a Tamagotchi, where players must care for and feed their virtual pets to keep them alive. In this proof of concept, users are tasked with the responsibility of consistently nourishing their Zen Token NFT (NFT citizen) to prevent its demise.

How it's Constructed
This project incorporates several technological components:

Magic Connect SDK
A fundamental Solidity contract
React
Once the user has authenticated via Magic, they gain the ability to interact with their NFT through the "feed" transaction. The "feed" action updates the "lastFed" parameter, which plays a crucial role in determining whether there is enough sustenance remaining for the NFT citizen's survival. The calculation is based on the equation: Food remaining = maxFood - foodConsumptionRate * timeElapsedSinceLastFed.

For the purposes of this proof of concept, the contract currently references a global "lastFed" parameter. However, there are plans to promptly follow this prototype with the implementation of a genuine ERC721 contract.




