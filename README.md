# Bifrost Subgraph Developer Guide

Welcome to the Bifrost Subgraph! This document will guide you through creating, deploying, and querying this subgraph.

## Prerequisites

Before getting started, make sure you have:

- Registered a Bifrost account and obtained an API key.
  - Please visit one of the following links and fill out the form to apply for an API key:
    - [https://forms.gle/tijPPdW37hFX6QFG9](https://forms.gle/tijPPdW37hFX6QFG9)
- Installed the [Graph CLI](https://github.com/graphprotocol/graph-cli).
- Installed the [Yarn package manager](https://yarnpkg.com/).

## Creating a Subgraph

1. Choose a subgraph name in the format `<username>/<subgraph-name>`, for example, "alice/mysubgraph".
   - `<username>`: This is your username on Bifrost.
   - `<subgraph-name>`: This is the specific name you choose for your subgraph, which usually reflects the functionality of the subgraph or the smart contract it indexes.

2. Run the following command in your terminal, replacing `{apikey}` with your Bifrost API key obtained from the links above and `<username/subgraph-name>` with your chosen subgraph name:

```bash
graph create --node https://bitlayer.bfno.de/{apikey} <username/subgraph-name>
```

## Removing a Subgraph

If you need to remove a subgraph, run the following command in your terminal, replacing {apikey} with your Bifrost API key and <username/subgraph-name> with the name of the subgraph you want to remove:

```bash
graph remove --node https://bitlayer.bfno.de/{apikey} <username/subgraph-name>
```

## Deploying a Subgraph

Run the following command in your terminal to deploy your subgraph, replacing {apikey} with your Bifrost API key and <username/subgraph-name> with your subgraph name:

```bash
graph deploy --node https://bitlayer.bfno.de/{apikey} --ipfs https://bitlayer.bfno.de <username/subgraph-name>
```

## Querying a Subgraph

Once deployed, you can use the following endpoints to query your subgraph:

- GraphQL Endpoint:

```bash
https://bitlayer.bfno.de/{apikey}/subgraphs/name/<username/subgraph-name>/graphql
```

- API Endpoint:

```bash 
https://bitlayer.bfno.de/{apikey}/subgraphs/name/<username/subgraph-name>
```

Replace {apikey} with your Bifrost API key obtained from the links above and <username/subgraph-name> with your subgraph name.

You can now use the standard GraphQL query language to query your Subgraph.

## Support

If you have any questions or feedback, please contact our support team at support@bfno.de. We're here to help!

Happy subgraphing with Bifrost!
