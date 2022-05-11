# automated-nft-marketplace

The NFT Marketplace that creates and upload its own NFT in the marketplace using AI.

## Initial Setup
0> Install Node.Js from here [Node Js](https://nodejs.org/en/download/current/) (Current)  
1> Git Clone The Repo in your Desired Location.  
2> Open the project in VS Code.  
3> Open Terminal in VS Code by Clicking `Terminal`>`New Terminal`
(Located on Top Menu Bar)  
4> Install the Following Dependencies by running these commands on the same terminal.
```bash
npm install ethers hardhat @nomiclabs/hardhat-waffle \
ethereum-waffle chai @nomiclabs/hardhat-ethers \
web3modal @openzeppelin/contracts ipfs-http-client \
axios
```
4> And Now run
```bash
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
```

## Usage
-1> Install [Metamask Wallet](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn?hl=en) on your browser and do the initial setup.(Click on create Wallet in the Auto generated Webpage and Follow Along.), Now Click on Extension and switch the wallet server to `localhost 8545`, by clicking on drop down menu named `Ethereum Mainnet`.

![server](https://i.stack.imgur.com/PKoHe.png)
    
0> Open a Split Terminal by Clicking `Terminal`>`Split Terminal`
(Located on Top Menu Bar Again !)   
1> Two Terminals should Appear Now,
On First Run
```bash
# install using NPM or Yarn
npm install

# or

yarn
```
and
```bash
npx hardhat node
```
2> Few Accounts Will Appear (20), choose any one of them and copy the private key.  
3> Go to Metamask Extension, make sure you are on localhost server. Click on round icon top right and click `Import Account`

![wallet](https://metamask.zendesk.com/hc/article_attachments/360079624651/Screen_Shot_2020-12-14_at_9.09.54_AM.png)

Paste Your Private key and and Click `Import`.

![import](https://metamask.zendesk.com/hc/article_attachments/360079624631/Screen_Shot_2020-12-14_at_9.10.07_AM.png)

Your Current Account Should Have 10000 eth now.

WELL DONE!!  

## RUNNING The Project

1> Now on "SECOND"(from the two opened Before) Terminal write the following command to put contract on Blockchain.
```bash
npx hardhat run scripts/deploy.js --network localhost
```
Now Run the final GUI Project
```bash
npm run dev
```
Now Visit [http://localhost:3000/](http://localhost:3000/)

## License
[MIT](https://choosealicense.com/licenses/mit/)
