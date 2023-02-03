# ERC20 Benchmarks

Benchmarks for implementations of the ERC20 standard.

Note: When comparing, keep in mind that Solmate and Maple implements ERC-2612 permit so it's more fairt to compare them against OpenZeppelin Permit and not the raw OpenZeppelin implementation.

- [OpenZeppelin](https://github.com/OpenZeppelin/openzeppelin-contracts)
- [OpenZeppelin Permit](https://github.com/OpenZeppelin/openzeppelin-contracts)
- [Solmate](https://github.com/rari-capital/solmate)
- [Maple](https://github.com/maple-labs/erc20)

## Methods TODO

- [x] deploy
- [x] transfer
- [x] transferFrom
- [x] approve
- [x] totalSupply
- [x] balanceOf
- [x] allowance

## Deployment

How much gas to deploy the contract as is?

<!-- Start deploy Table -->
|       Implementation      |  --  |
|---------------------------|------|
|           Maple           |764894|
|OpenZeppelin Permit (draft)|948373|
|        OpenZeppelin       |650209|
|          Solmate          |729680|
<!-- End deploy Table -->

## Write methods

### transfer

How much gas to transfer tokens?

#### To a wallet that already owns a token

<!-- Start transferToOwner Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |20975|
|OpenZeppelin Permit (draft)|21239|
|        OpenZeppelin       |21195|
|          Solmate          |20869|
<!-- End transferToOwner Table -->

#### To a wallet that owns no token

<!-- Start transferToNonOwner Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |38053|
|OpenZeppelin Permit (draft)|38317|
|        OpenZeppelin       |38273|
|          Solmate          |37947|
<!-- End transferToNonOwner Table -->

### transferFrom

How much gas to transfer tokens?

#### To a wallet that already owns a token

<!-- Start transferFromToOwner Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |28116|
|OpenZeppelin Permit (draft)|28457|
|        OpenZeppelin       |28457|
|          Solmate          |26207|
<!-- End transferFromToOwner Table -->

#### To a wallet that owns no token

<!-- Start transferFromToNonOwner Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |45238|
|OpenZeppelin Permit (draft)|45579|
|        OpenZeppelin       |45579|
|          Solmate          |43329|
<!-- End transferFromToNonOwner Table -->

### approve

How much gas to approve an address to spend some amount of tokens?

<!-- Start approve Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |32772|
|OpenZeppelin Permit (draft)|32885|
|        OpenZeppelin       |32885|
|          Solmate          |32720|
<!-- End approve Table -->

## View methods

How much gas to check the total supply of tokens?

### totalSupply

<!-- Start totalSupply Table -->
|       Implementation      | -- |
|---------------------------|----|
|           Maple           |7548|
|OpenZeppelin Permit (draft)|7548|
|        OpenZeppelin       |7548|
|          Solmate          |7548|
<!-- End totalSupply Table -->

### balanceOf

How much gas to check the balance of a wallet?

<!-- Start balanceOf Table -->
|       Implementation      | -- |
|---------------------------|----|
|           Maple           |7849|
|OpenZeppelin Permit (draft)|7830|
|        OpenZeppelin       |7808|
|          Solmate          |7805|
<!-- End balanceOf Table -->

### allowance

How much gas to check gow much a wallet can spend on behalf of another wallet?

<!-- Start allowance Table -->
|       Implementation      | -- |
|---------------------------|----|
|           Maple           |8145|
|OpenZeppelin Permit (draft)|8123|
|        OpenZeppelin       |8057|
|          Solmate          |8079|
<!-- End allowance Table -->
