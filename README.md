# Graph node for MVM Mainnet

Host: [https://graph.mvg.finance](https://graph.mvg.finance)


## Subgraph deployment

Deploy the subgraph to the node:
```
1. Prepare the subgraph first (Edit the subgraph.yaml)

- [ ] Edit contract `address` to your MVM contract address
- [ ] Edit `network` to `mainnet`

2. Build and deploy

$ graph codegen

$ graph build

$ graph create --node https://graph.mvg.finance/deploy [YOUR GRAPH NAME]

$ graph deploy --ipfs http://graph.mvg.finance:5001 --node https://graph.mvg.finance/deploy [YOUR GRAPH NAME]

3. Test your subgraph through visiting https://graph.mvg.finance/subgraphs/name/[YOUR GRAPH NAME]
```

Deploy guide:
- [deploy-the-subgraph](https://github.com/graphprotocol/graph-node/blob/master/docs/getting-started.md#24-deploy-the-subgraph)
- [subgraph-manifest](https://github.com/graphprotocol/graph-node/blob/master/docs/subgraph-manifest.md)

## About the set up of the node
Use docker to run the node: https://medium.com/coinmonks/deploy-subgraphs-to-any-evm-aaaccc3559f

To enable https, use nginx for proxy, generate conf: https://www.digitalocean.com/community/tools/nginx

Hardware: 
- 4 vCPU
- 16GB RAM
- 1TB HDD

