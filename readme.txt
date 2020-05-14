Project Summary: 

An elections application for A select few of the candidates that were running in the democratic primaries

-----------------------------------------------------------------------------------------------------------------

Technology Stack:

- Front end UI built with HTML, bootstrap, javaScript, CSS
- Mediator/ Glue between UI and EVM: Web3
- Blockchain: Ethereum with Ethereum Virtual Machine
- Compiler : truffle
- Ethereum Blockchain manager/ networ : Ganache

-----------------------------------------------------------------------------------------------------------------

Dependencies Installation:

- Install Node or Node Package manager
- Install truffle: npm install -g truffle
- Ganache
    The next dependency is Ganache, a local in-memory blockchain. You can install Ganache by downloading 
    it from the Truffle Framework website. It will give us 10 external accounts with addresses on our local 
    Ethereum blockchain. Each account is preloaded with 100 fake ether.
- MetaMask Install MetaMask, create an account and connect to the Ethereum network running on localhost

-----------------------------------------------------------------------------------------------------------------

How To Run:

** The Project already contains compiled code **
- Open Chrome Browser
- cd to project directory then type in cmd or terminal 
    : npm install
    : npm run dev
- You will be provided with local host url and browser should be automatically launched

- running tests: truffle tests
- compiling: truffle migrate --reset

-----------------------------------------------------------------------------------------------------------------

Using the Voting dapp:
    Only one account can vote at a time so after you vote, the vote button will disapper.
    Inorder to vote again, swich accounts in MetaMask, Multiple accounts can be imported
    from Ganache.
    Note: MetaMask and chrome is glichy so refresh inbetween actions when page is loading ...

------------------------------------------------------------------------------------------------------------------

Project Structure:

--build
|______Election.json (compiled election dapp byte code for evm)
|______Migration.json (came with project starter please ignore)

--contracts
|______Election.sol (solidity smart contracts)
|______Migration.sol (came with project starter please ignore)

--migrations
|______1_initial_migration.js (came with project starter please ignore)
|______2_initial_migration.js (Complitation strategy for smart contracts)

--src (web components)
|______js
|______|______app.js (javascript code for UI)
|______index.html (Elections UI)

--test (Project tests for smart contracts)
|______election.js
