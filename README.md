# sample-subgraph
sample-subgraph

### usage
##### install OpenZeppelin in local project
```
npm install @openzeppelin/subgraphs
```
```
yarn
```

##### build and deploy subgraph
configs/sample.json describes a erc20-subgraph, it can be compiled by:
```
yarn compiler-erc20 
yarn build-erc20
yarn codegen-erc20
yarn create-erc20-local
yarn deploy-erc20-local
```
> yarn CMD is defined in package.josn

> for details refer docs/*


##### sample.json
```
{
  "output": "generated/sample.",
  "chain": "dev",
  "id": "erc20",
  "startBlock": "12000000",
  "datasources": [
    {
      "module": [
        "erc20"
      ]
    }
  ]
}
```

* id: subgraph name
* startBlock: subgraph original position
* module: load "erc20""module" from src/datasources/erc20.yaml
