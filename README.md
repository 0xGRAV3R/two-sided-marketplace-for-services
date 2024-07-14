# two-sided-marketplace-for-services

Using Anchor, create a 2-sided marketplace model for services. Vendors should be able to list services, with service agreements represented by metadata in NFTs. Consumers should be able to purchase service NFTs. The marketplace should support soulbound and non-soulbound NFTs and collect royalties on resales.<br><br>

-Develop a 2-sided marketplace using Anchor.<br>
-Allow vendors to list services as NFTs.<br>
-Enable consumers to purchase service NFTs.<br>
-Support soulbound and non-soulbound NFTs, with royalty collection for resales.

## Getting Started

### Prerequisites

- Node v18.18.0 or higher

- Rust v1.77.2 or higher
- Anchor CLI 0.30.0 or higher
- Solana CLI 1.18.9 or higher

### Installation

#### Clone the repo

```shell
git clone https://github.com/0xGRAV3R/whitelist-gated-token-sale.git
cd whitelist-gated-token-sale
```

#### Install Dependencies

```shell
npm install
```

#### Start the web app

```
npm run dev
```

## Apps

### anchor

This is a Solana program written in Rust using the Anchor framework.

#### Commands

You can use any normal anchor commands. Either move to the `anchor` directory and run the `anchor` command or prefix the command with `npm run`, eg: `npm run anchor`.

#### Sync the program id:

Running this command will create a new keypair in the `anchor/target/deploy` directory and save the address to the Anchor config file and update the `declare_id!` macro in the `./src/lib.rs` file of the program.

You will manually need to update the constant in `anchor/lib/counter-exports.ts` to match the new program id.

```shell
npm run anchor keys sync
```

#### Build the program:

```shell
npm run anchor-build
```

#### Start the test validator with the program deployed:

```shell
npm run anchor-localnet
```

#### Run the tests

```shell
npm run anchor-test
```

#### Deploy to Devnet

```shell
npm run anchor deploy --provider.cluster devnet
```

### web

This is a React app that uses the Anchor generated client to interact with the Solana program.

#### Commands

Start the web app

```shell
npm run dev
```

Build the web app

```shell
npm run build
```

