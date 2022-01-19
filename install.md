1. git clone https://github.com/esrdapp/tokenbridge-contracts.git
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
13. update the deploy/src/deploymentUtils.js file on lines 125 & 139 if necessary (currently supports HPB network chain 269)
14. cd ..
15. docker-compose up -d --build
16. ./deploy.sh
17. make note of home and foreign bridge contracts for oracle deployment

example successfull deployment:

Deployment of Arbitrary Message Bridge at Foreign completed


Deployment has been completed.


[   Home  ] HomeBridge: 0x12d9DFD6F845c20DB6220dbDEB32FAD12dc528AD at block 13548847
[ Foreign ] ForeignBridge: 0x06188d65DF1C18b1E7d29e5D34bF8cc9aEa0E866 at block 20189894
Contracts Deployment have been saved to `bridgeDeploymentResults.json`
{
    "homeBridge": {
        "address": "0x12d9DFD6F845c20DB6220dbDEB32FAD12dc528AD",
        "deployedBlockNumber": 13548847
    },
    "foreignBridge": {
        "address": "0x06188d65DF1C18b1E7d29e5D34bF8cc9aEa0E866",
        "deployedBlockNumber": 20189894
    }
}


