# Pokémon Storage System

The Pokèmon Storage System (PSS) allows trainers to store their own Pokemon without the need to carry them in the current team. It was originally developed by the Japanese researcher Masaki Sonezaki,known in the West as [Bill](https://bulbapedia.bulbagarden.net/wiki/Bill), ???, Someone or Satoshi Nakamoto.

The original implementation of PSS was improved by other scientists but the functionality has not changed over time.

PSS is a decentralised ledger that stores the ownership of Pokémon in 'boxes' and allows to move the owned ones in and out from the team. 
As a forerunner Blockchain system, the first version required the trainer to access it through full nodes, usually located in the proximity of Pokémon Centers. Newer versions (e.g. Pokémon Box in Pokémon Go) are made portable because of the use of sharding or a lighting network.
The original system was able to store only a limited account of Pokemon per trainer. To cope with this lack of scalability  there were introduced more boxes per PSS. 

Here we propose a simple implementation of PSS using a Solidity smart contract and the Solitude development tool.

![PSS](media/bill_blockchain.png?raw=true "Bill PSS implementation")

The contract will implement the following methods:

- Get: For getting the list of owned Pokemon in a specific box 
- Withdraw: For moving into the Team Pokemon that were prior deposited into the system
- Deposit: To move out Pokemon from the team to the decentralised system
- Release: For removing the ownership of Pokemon and make them wild and free again
- Change Box: For setting the current box 
