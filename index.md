## Welcome to BitcoinEco

Where ecology meets economics.  bitcoinEco is the entire Bitcoin system run in a smart contract where you will be able to earn by staking your BitcoinEco.

### Tokenomics

BitcoinEco tokenomics mirrors Bitcoin with an ERC-20 Token which has minted to a legacy address, this address pays out BTCECO to deligaters proportionally to theyre stake every 5 days. These rewards are halved according to Bitcoins halving cycle.



    constructor() public {
        name = "BitcoinEco";
        symbol = "BTCECO";
        decimals = 8;
        _totalSupply = 2100000000000000;

        balances[msg.sender] = _totalSupply;
        emit Transfer(address(0), msg.sender, _totalSupply);
    }
