1- cloner le dépôt avec la commande : git clone https://github.com/stean985/CoreDao-Dapp1-Fr.git

2- naviguez dans le repertoire : cd /CoreDao-Dapp1/Backend
3- créé-y un fichier json avec pour nom : secret.json
4- ouvrez le fichier secret.json et collez-y la ligne ci-dessous :
{"PrivateKey":"la clé privée de votre wallet portefeuille électronique"}


5- installez les dépendances Hardhat avec la commande : npm install --save-dev hardhat
6- compilez le contrat intellignet Storage.sol avec la commande : npx hardhat compile
7- et enfin déployer le contrat intelligent avec la commande : npx hardhat run ./scripts/deploy-and-call.js
le résultat va ressembler à ceci :

>npx hardhat run scripts/deploy-and-call.js
Storage contract deployed to: 0x48F68BF4A1b1fE6589B9D0a5ad0dF0520582edA2
call retrieve(): BigNumber { value: "0" }
call store(), set value to 100
call retrieve() again: BigNumber { value: "100" }


8- naviguez dans le repertoire : cd /CoreDao-Dapp1/Frontend
9- installez toutes les dépendances (exemple les modules Node.js) avec la commande : npm install
10- testez le projet avec la comande : npm run dev
