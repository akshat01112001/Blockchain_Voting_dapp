# Blockchain_Voting_dapp

Current voting systems like ballot box voting or electronic voting suffer from 
various security threats such as DDoS attacks, polling booth capturing, 
vote alteration and manipulation, malware attacks, etc, and also require 
huge amounts of paperwork, human resources, and time. This creates a 
sense of distrust among existing systems.

In this decentralized application we create a mechanism for e-voting based 
on Blockchain. The website works as follows. At first an election is created 
by the admin. Then the admin adds candidates by taking their inputs. This
list can then be viewed by clicking on the view candidates button.

![ox52tih](https://user-images.githubusercontent.com/76171905/206509868-dfce7fe7-6f88-44d1-9309-3ca2484aabe2.png)


After that the user registers the voters by taking their inputs. This list can 
also be viewed.
Adding both these bunch of data on the Blockchain will cost some gas and 
the same will be paid by the admin account from Ganache.
After taking data about both the candidate and the voter, the admin can 
then begin the voting process

<img width="710" alt="brave_RE0yFX6olO" src="https://user-images.githubusercontent.com/76171905/206509680-1e81910e-2ac4-407a-a39d-0373cb4b121e.png">

Each voter is linked with one account from Ganache and provisions have 
been made to make sure that only one vote can be casted from one 
account.
After all accounts have casted their votes, the admin then closes the 
election and declares the result, which is displayed in order of their votes.
In the solidity code, there are two structs, one for candidates and one for 
voters.
Then there is mapping for candidates and voters. 
The backend links the solidity code with the front end in HTML/CSS 

<img width="877" alt="brave_iVqvfvTySA" src="https://user-images.githubusercontent.com/76171905/206510092-e9991d5c-867b-4456-b695-dba0aa702d1d.png">

## Dependencies
Install these prerequisites 
- NPM: https://nodejs.org
- Truffle: https://github.com/trufflesuite/truffle
- Ganache: http://truffleframework.com/ganache/
- Metamask: https://metamask.io/


## Step 1. Clone the project

## Step 2. Install dependencies
```
$ cd election
$ npm install
```
## Step 3. Start Ganache
Open the Ganache GUI client that you downloaded and installed. This will start your local blockchain instance.

## Step 4. Compile & Deploy Election Smart Contract
`$ truffle migrate --reset`
You must migrate the election smart contract each time your restart ganache.

## Step 5. Configure Metamask
- Unlock Metamask
- Connect metamask to your local Etherum blockchain provided by Ganache.
- Import an account provided by ganache.

## Step 6. Run the Front End Application
`$ npm run dev`
Visit this URL in your browser: http://localhost:3000

