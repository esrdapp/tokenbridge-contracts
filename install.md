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


