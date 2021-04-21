## fintech_hw_20

We were tasked with writing a simple smart contract that allows for profit splitting of amounts sent to a specific contract address. 

Here we'll be using Remix IDE, Ganache, and Metamask to test out our contract on the local private test network.

Here we have a very basic smart contract that is going to take 3 inputs (employee addresses), take any amount sent to the contract, split it into 3, and then send out the equal parts to each employee. We made sure to match our compiler to our version of solidity to minimize any errors in compiling. Once the contract is written, we compile it. 
<br>
![Screenshot1](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS1.png)
<br>
Next we want to deploy the smart contract onto a test network. In this case we setup metamask to connect with our local network. By hitting deploy (currently hidden above the transact button) we will deploy our contract to the network for the cost of the current network fee (see as GAS FEE in the metamask extension). It's also good to note that in this case we've input the variables of employee addresses in the lefthand side of remix. 
<br>
![Screenshot2](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS4%20-%20Deploying%20Contract.png)
<br>
Here we open up Ganache and demonstrate the balances pre-contract testing (notice that we've tested this once already before screenshotting.)
<br>
![Screenshot3](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/Hw20SS3%20-%20PreTransaction.png)
<br>
Next we are going to test sending a specific amount to our contract by selecting deposit in the bottom left unders deployed contracts. This will cost us 15ETH plus gas.

<br>
![Screenshot5](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS5%20-%20Testing%20Deposit.png)
<br>
Finally we can see that the contract executed successfully and we ended up with +5ETH in each of our employee addresses. 
<br>
![Screenshot6](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS6%20-%20Wallets%20After.png)
<br>
We can also look at the Tx Hash to verify that the from address sent 15ETH to the Contract Address and not individually to the employee wallets. 
![Screenshot7](https://github.com/MedakaRiceFish/fintech_hw_20/blob/main/Screenshots/hw20SS7%20-%20Tx%20Hash.png)
