# Introduction

The front-end of OpenBook is implemented with Next.js, which is a web development framework that is built on top of the React framework. Since this is a react framework, everything is a component with its own states. To communicate between different components, OpenBook utilizes a React library called Redux. Redux is for managing and centralizing application state. In the case of OpenBook, Redux is responsible for storing and managing the odds data, the web3 related data, the liquidity data, the betslip states, and the bets data. Redux states are updated whenever the smart contracts emit events and all the front-end components are updated accordingly. Hence there is no refresh needed, which provides excellent user experience. To further improve user experience, an additional library called Redux Persist is used.  Redux Persist is responsible for storing relevant redux states in localstorage, such as games picked and games favorited. The OpenBook DAPP is divided into four parts, the side and top navigation, the betting page, the account page and the bookie page. The following sections will explain each part, and how the UI components are mapped to the smart contract functions.

![](https://lh3.googleusercontent.com/XljeMk-9QpqyGx3x3ebBV8j-Po5ApvoRgv9-KgtvG3jt4NxT4TbfyIPjR2bTGWNMMm99Z4ZYU7W5xbtiUQ9SRbx8ZTRmj8B1KBFyrESHO70SGPnLcFdC5\_zAF-xiEIhocRwmWm5m1TQm013k)![](https://lh3.googleusercontent.com/oiwSSgUaLVwp90odCF4QPLg-y-3XLVUXDz0KU32DKxlwRUhsuNPVENyRUCLXXsO8Lbmb55Ac8eqktLz6KTGrdpaawlSBc8tx0nwkbpKIf0GsXWzPvMQTPKgHnpV9OeuRu\_eIPmZdDhqJlIaN)