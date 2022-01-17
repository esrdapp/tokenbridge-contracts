1. git clone
2. node --version             // used v10.19.0 - easy to switch with Node Version Manager (NVM -https://github.com/nvm-sh/nvm)
3. npm --version              // used v6.14.4
4. cd tokenbridge-contracts
5. npm install
6. npm audit fix  
7. npm install 
8. npm run compile
9. cd deploy
10. mv .env.example .env
12. update addresses and private key of .env file
13. cd ..
14. ./deploy.sh

deploying storage for home validators
Error: web3 RPC failed: {"code":-32000,"message":"invalid sender"}
    at sendNodeRequest (/contracts/deploy/src/deploymentUtils.js:161:9)
    at process._tickCallback (internal/process/next_tick.js:68:7)
Error: TypeError: Cannot read property 'status' of undefined
    at deployContract (/contracts/deploy/src/deploymentUtils.js:63:32)
    at process._tickCallback (internal/process/next_tick.js:68:7)


