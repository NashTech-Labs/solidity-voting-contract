# solidity-voting-contract
This smart contract is a small voting contract that wil demonstrate the voting system. The main problems of electronic voting is how to assign voting rights to the correct persons and how to prevent manipulation. This smart contract will not solve all problems, but at least it will show how delegated voting can be done so that vote counting is automatic and completely transparent at the same time.

The idea is to create one contract per ballot, providing a short name for each option. Then the creator of the contract who serves as chairperson will give the right to vote to each address individually.

The persons behind the addresses can then choose to either vote themselves or to delegate their vote to a person they trust.

At the end of the voting time, _winningProposal_() will return the proposal with the largest number of votes.

### Deploy and Testing

You can deploy this contract on _https://remix.ethereum.org/_ and then test it using the **voting-test.sol** contract on remix.
