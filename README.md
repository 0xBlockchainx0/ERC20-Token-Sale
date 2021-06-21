

[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



# ERC20 Token Creation and Crowd Sale

Utilising the Truffle framework to test and deploy the token, this repo also contains a rudimentary front end, built with React, that allows users to 'buy' tokens in a crowd sale fashion. Said token has been deployed and tested on the Ropsten and Goerli networks.
   



### Real-World Use-Cases


💰 Tokenization of any assets as fungible tokens (ERC20)

🏦 Creation of bonus programs, vouchers, etc

💲 Creation of a new crypto currency

🧾 Creation of a payment-layer on top of Ethereum


### Development-Goals


🧰 Develop deeper understanding of truffle-config files

🤖 Understand deployment of dApps

🦸‍♂️ Understand tokenization using Open-Zeppelin Smart Contracts

☑️ Deeper dive into unit-testing




## Built With

* [Truffle](https://www.trufflesuite.com/)
* [React](https://reactjs.org/)
* [Open Zeppelin](https://openzeppelin.com/)
* [Mocha](https://mochajs.org/)
* [Chai](https://www.chaijs.com/)
* [Web3js](https://web3js.readthedocs.io/en/v1.3.4/)
* [Node.js](https://nodejs.org/en/)


<!-- GETTING STARTED -->
## Getting Started

1. Enter the inital token supply and your wallet mnemonic in the env file
  ```sh
   INITIAL_TOKENS=
   MNEMONIC=
  ```
   
2. If looking to deploy on ETH test networks then enter the relevant URL path for your web3 connection in the truffle-config.js file ([Infura](https://infura.io/) was used for this project)
  ```JS
   goerli_infura: {
      provider: function() {
        return new HDWalletProvider(process.env.MNEMONIC, "INSERT web3 PROVIDER ADDRESS HERE", AccountIndex)
      },
      network_id: 5
    },
    ropsten_infura: {
      provider: function() {
        return new HDWalletProvider(process.env.MNEMONIC, "INSERT web3 PROVIDER ADDRESS HERE", AccountIndex)
      },
      network_id: 3
    }
   ```
   
3. To run the front end locally (at http://localhost:3000), ensure you are in the "client" directory and use a terminal to execute the following
  ```bash
  npm run start
  ```
  
<p align="center">
  <img width="777" height="393" src="/screenshot.png">
</p>

  

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Twitter - [@TraderTDF](https://twitter.com/TraderTDF)

LinkedIn - [https://www.linkedin.com/in/RAMWatson/](https://www.linkedin.com/in/RAMWatson/)

Project Link: [https://github.com/Elisik/ERC20-Token-Sale](https://github.com/Elisik/ERC20-Token-Sale)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
This project was created as part of the Ethereum Blockchain Developer Bootcamp as linked below.
* [Ethereum Blockchain Developer Bootcamp With Solidity (2021)](https://www.udemy.com/course/blockchain-developer/)




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/RAMWatson/
[product-screenshot]: screenshot.jpg
