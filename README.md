# C3 DApp supply chain solution backed by the Ethereum platform
**PROJECT: DApp supply chain solution backed by the Ethereum platform**

### Part 1: write-ups
Project submitted on 12/11/2021

#### 1. UML in UML folder for coffee supply chain
in UML\
#### 2. Libraries
in project-6\node_modules
```bash
# Node v12.0.0
# npm v6.9.0
# Truffle v4.1.14 (core: 4.1.14)
# Solidity v0.4.24 (solc-js)
```
#### 3. IPFS
Not used so far

### Part 2: write smart contracts

#### 1. Define and implement required interfaces
#### 2. Build out AccessControl Contracts
in project-6\contracts\coffeeaccesscontrol\
#### 3. Build out Base Contract
in project-6\contracts\coffeebase\
#### 4. Build out Core Contract
in project-6\contracts\coffeecore\

### Part 3: Test smart contract code coverage

#### 1. Test every function
![Test results: ](https://github.com/quidba7/blockchain_project_3/project-6/pictures/test.PNG)

### Part 4: Deploy smart contracts on public test network

#### 1. Deploy
We successfuly deployed our contract to rinkeby test network
![rinkeby deployment: ](https://github.com/quidba7/blockchain_project_3/project-6/pictures/rinkeby_deployment.PNG)
#### 2. Submit contract address
We only show contract and transaction hash of the SupplyChain contract.
    - contract SupplyChain ['0x73ec3678b892ab7239f636475463ff8da4696e8f'](https://rinkeby.etherscan.io/address/0x73ec3678b892ab7239f636475463ff8da4696e8f)
    - transaction for deploying SupplyChain: ['0xf41cc443fddc569bc913e1589d8ca047d1e93d3ad25f300fb03f865b95f79e9d']https://rinkeby.etherscan.io/tx/0xf41cc443fddc569bc913e1589d8ca047d1e93d3ad25f300fb03f865b95f79e9d)

### Part 5: Modify client code to interact with smart contract

#### 1. Configure client code for each actor
1) Submit a product for shipment (farmer to the distributor, distributor to retailer, etc).
Submit a product for shipment transaction ['0x8003fae0d0b46c5c564fef0457b55c69cbcd42c541809d3ca8e3575dd551e2be'](https://rinkeby.etherscan.io/tx/0x8003fae0d0b46c5c564fef0457b55c69cbcd42c541809d3ca8e3575dd551e2be)
2) Receive product from shipment.
Receive product ['0xa1f0e58de9680e8b94ee37693eeaa259602edcd3d28e37ad2ef788632e9869f2'](https://rinkeby.etherscan.io/tx/0xa1f0e58de9680e8b94ee37693eeaa259602edcd3d28e37ad2ef788632e9869f2)
3) Validate the authenticity of the product.

fetchItemBufferOne
```bash
    8) [X, X, '0x18bd4e3354e0d99d06ffded10793eec71debc9e3', '0x18bd4e3354e0d99d06ffded10793eec71debc9e3', 'John Doe', 'Yarra Valley', '-38.239770', '144.341490']
    0: X {s: 1, e: 0, c: Array(1)}
    1: X {s: 1, e: 0, c: Array(1)}
    2: "0x18bd4e3354e0d99d06ffded10793eec71debc9e3"
    3: "0x18bd4e3354e0d99d06ffded10793eec71debc9e3"
    4: "John Doe"
    5: "Yarra Valley"
    6: "-38.239770"
    7: "144.341490"
    length: 8
```

fetchItemBufferTwo
```bash
    0: X {s: 1, e: 0, c: Array(1)}
    1: X {s: 1, e: 0, c: Array(1)}
    2: X {s: 1, e: 0, c: Array(1)}
    3: "Best beans for Espresso"
    4: X {s: 1, e: 0, c: Array(1)}
    5: X {s: 1, e: 0, c: Array(1)}
    6: "0x18bd4e3354e0d99d06ffded10793eec71debc9e3"
    7: "0x18bd4e3354e0d99d06ffded10793eec71debc9e3"
    8: "0x18bd4e3354e0d99d06ffded10793eec71debc9e3"
    length: 9
```

### Part 6: Optional: Implement Infura to store product image
