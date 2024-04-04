## Arweave transaction cost analysis

### Goal
The purpose of this analysis is to better understand Arweave's transaction fee mechanism, by analyzing real transaction cost per byte over the ~1yr timeline. 

The analysis is used in a blog post discussing the cost of using speculative project tokens to denominate user/developer actions in web3 project. 

### Arweave transaction data 
The information is retrieved with a graphql query run on an Arweave gateway that is hosted by ar.io. 

The gateway is offered for free to the Arweave community. The gateway's resources are appropriately restricted, which makes getting enough data for proper time series analysis difficult. 

To work around this, the query pulls back a sample of random blocks from the last ~9 months. 

### Files
arweave_txs notebook contains the query
arweave_txs_analysis reads the query results and has the resulting analysis
