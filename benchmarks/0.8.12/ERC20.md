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
|           Maple           |763681|
|OpenZeppelin Permit (draft)|953786|
|        OpenZeppelin       |655622|
|          Solmate          |733694|
<!-- End deploy Table -->

## Write methods

### transfer

How much gas to transfer tokens?

#### To a wallet that already owns a token

<!-- Start transferToOwner Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |20978|
|OpenZeppelin Permit (draft)|21269|
|        OpenZeppelin       |21225|
|          Solmate          |20869|
<!-- End transferToOwner Table -->

#### To a wallet that owns no token

<!-- Start transferToNonOwner Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |38056|
|OpenZeppelin Permit (draft)|38347|
|        OpenZeppelin       |38303|
|          Solmate          |37947|
<!-- End transferToNonOwner Table -->

### transferFrom

How much gas to transfer tokens?

#### To a wallet that already owns a token

<!-- Start transferFromToOwner Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |28119|
|OpenZeppelin Permit (draft)|28496|
|        OpenZeppelin       |28496|
|          Solmate          |26283|
<!-- End transferFromToOwner Table -->

#### To a wallet that owns no token

<!-- Start transferFromToNonOwner Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |45241|
|OpenZeppelin Permit (draft)|45618|
|        OpenZeppelin       |45618|
|          Solmate          |43405|
<!-- End transferFromToNonOwner Table -->

### approve

How much gas to approve an address to spend some amount of tokens?

<!-- Start approve Table -->
|       Implementation      |  -- |
|---------------------------|-----|
|           Maple           |32772|
|OpenZeppelin Permit (draft)|32894|
|        OpenZeppelin       |32894|
|          Solmate          |32744|
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
