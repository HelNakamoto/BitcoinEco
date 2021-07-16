## Welcome to BitcoinEco

[Exchange](https://app.uniswap.org/#/swap?exactField=input&exactAmount=10&use=v1&outputCurrency=0xf28B5eBC98bE9a7D58269C782938180DdE3B40Ed)

[Etherscan](https://etherscan.io/token/0xf28b5ebc98be9a7d58269c782938180dde3b40ed)

Contract: 0xf28B5eBC98bE9a7D58269C782938180DdE3B40Ed

Where ecology meets economics.  bitcoinEco is the entire Bitcoin system run in a smart contract where you will be able to earn by staking your BitcoinEco.

### Tokenomics

The BitcoinEco tokenomics mirror Bitcoin with an ERC-20 Token which has minted to a genesis address,  this address pays BTCECO to delegators proportionally to the amount staked every 5 days.  these rewards are halved according to Bitcoins halving cycle.



    constructor() public {
        name = "BitcoinEco";
        symbol = "BTCECO";
        decimals = 8;
        _totalSupply = 2100000000000000;

        balances[msg.sender] = _totalSupply;
        emit Transfer(address(0), msg.sender, _totalSupply);
    }
