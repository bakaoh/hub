# Monkeyfile reference

A `Monkeyfile` is a text document that contains all the commands a user could call on web3 to deploy an decentralized application.

This page describes the commands you can use in a `Monkeyfile`.

## Usage

The `MonkeyEngine` runs the instructions in the `Monkeyfile` one-by-one, sending the transaction to rpc endpoint if necessary, before finally outputting the addresses of your new contracts.

## Format

Here is the format of the `Monkeyfile`:

```
# Comment
INSTRUCTION arguments
[argument]
[argument]
```

The instruction is case-sensitive. `MonkeyEngine` runs instructions in a `Monkeyfile` in order. `Monkeyfile` treats lines that begin with `#` as a comment.

List of instructions in the `Monkeyfile`:

- FROM
- PARAM
- DEPLOY
- RUN

### FROM

```
FROM <monkey id>
```

### PARAM

```
PARAM <name> <type>
<default value>
```

### DEPLOY

```
DEPLOY <name>
<bytecode>
<abi>
<paramenters>
```

### RUN

```
RUN <contract>
<method>
<paramenters>
```
