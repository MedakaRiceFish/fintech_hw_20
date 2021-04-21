## fintech_hw_20

We were tasked with writing a simple smart contract that allows for profit splitting of amounts sent to a specific contract address. 

Starting Testnet Address: 0x067e1064A2Df01bB917Ed79b27ab359990471Bbd
<p>
Contract Address: 0xb64Cb5e58C634d685f8B27DdDDBA0E08e5Af2A8E


Here we'll be using Remix IDE, Ganache, and Metamask to test out our contract on the local private test network.

Here we have a very basic smart contract that is going to take 3 inputs (employee addresses), take any amount sent to the contract, split it into 3, and then send out the equal parts to each employee. We made sure to match our compiler to our version of solidity to minimize any errors in compiling. Once the contract is written, we compile it. 

<p>
  
![Screenshot1](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS%20-%20updated.png)

<p>

Next we want to deploy the smart contract onto a test network. In this case we setup metamask to connect with our local network. By hitting deploy (currently hidden above the transact button) we will deploy our contract to the network for the cost of the current network fee (see as GAS FEE in the metamask extension). It's also good to note that in this case we've input the variables of employee addresses in the lefthand side of remix. 

<p>
  
![Screenshot2](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS4%20-%20Deploying%20Contract.png)

<p>

Here we open up Ganache and demonstrate the balances pre-contract testing (notice that we've tested this once already before screenshotting.)

<p>

![Screenshot3](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/Hw20SS3%20-%20PreTransaction.png)

<p>

Next we are going to test sending a specific amount to our contract by selecting deposit in the bottom left unders deployed contracts. This will cost us 15ETH plus gas.

<p>
  
![Screenshot5](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS5%20-%20Testing%20Deposit.png)

<p>
  
  
Finally we can see that the contract executed successfully and we ended up with +5ETH in each of our employee addresses. 

<p>

![Screenshot6](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS6%20-%20Wallets%20After.png)

<p>

We can also look at the Tx Hash to verify that the from address sent 15ETH to the Contract Address and not individually to the employee wallets. 

<p>

![Screenshot7](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS7%20-%20Tx%20Hash.png)


Ropsten Test Net: https://ropsten.etherscan.io/tx/0xddddcf24763014df663e3832d53b86f0a90161a6163c11a49ef68c80c2e3f25c

Ropsten Deployment Proof:

![Ropsten1](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS%20-%20Ropsten%20Deploy.png)
