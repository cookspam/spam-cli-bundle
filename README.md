# Spam Bundle CLI

A command line interface for the Spam program (max 5 transactions per single RPC call).

## Building

To build the Spam CLI, you will need to have the Rust programming language installed. You can install Rust by following the instructions on the [Rust website](https://www.rust-lang.org/tools/install).

Once you have Rust installed, you can build the Spam CLI by running the following command:

```sh
cargo build --release
```

## Usage

## Mining Spam

To mine spam, use the command below. Replace $RPC_URL with your Solana RPC URL and $KEY_PATH with the path to your keypair file. **You can use max 5 keypairs:

You can mine spam by running the following command:

```sh
cargo run --release -- --rpc $RPC_URL --keypair1 $KEY_PATH1  --keypair2 $KEY_PATH2 --keypair3 $KEY_PATH3 --keypair4 $KEY_PATH5 --keypair5 $KEY_PATH5 mine
```

If the mining process fails on the first attempt, try running the command again.

## Checking Claimable Rewards

To check your claimable rewards, use the following command:

```sh
cargo run --release -- --rpc $RPC_URL --keypair1 $KEY_PATH1  --keypair2 $KEY_PATH2 --keypair3 $KEY_PATH3 --keypair4 $KEY_PATH5 --keypair5 $KEY_PATH5 rewards
```

## Claiming Spam

To claim your mined spam, run:

```sh
cargo run --release -- --rpc $RPC_URL --keypair1 $KEY_PATH1  --keypair2 $KEY_PATH2 --keypair3 $KEY_PATH3 --keypair4 $KEY_PATH5 --keypair5 $KEY_PATH5 claim
```

# Troubleshooting
+ Ensure that your Solana RPC URL and keypair file path are correctly specified.
+ If you encounter issues during mining, retry the command as network conditions may vary.

For further assistance, please refer to the official documentation or contact the support team.
