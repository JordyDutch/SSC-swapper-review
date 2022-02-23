# SSC Swapper

Hello SSC team, Lumenous and I tested the [SSC swapper](https://swapper.silesia.network/) and found/suggest the following things:

## BUGS

#### Rinkeby explorer problem
-----
- Swapper is showing "view explorer" and opens Kovan testnet while transactions were on Rinkeby testnet. When you open the explorer from metamask you will be redirected to Rinkeby and you see your transaction.
<br />

[Screenshot swapper transaction](https://github.com/JordyDutch/images/blob/main/Swapper.png?raw=true)
<br />
[Screenshot Kovan explorer](https://github.com/JordyDutch/images/blob/main/Kovan%20explorer%20link-Rinkeby.png?raw=true)

- The transaction link returns no transaction on etherscan

###### Rinkeby sends you to Kovan

[transaction id](https://kovan.etherscan.io/tx/0x6e125ea5a8faad865fc34155b6abb2579e5d8f69b8d6fc86422dc0cfa225badc)

###### Kovan send you to Ropsten
[transaction id](https://ropsten.etherscan.io/tx/0xcfb89fc1cca2f39c8f85210df072b15c869fa83bee6ba0becc1edd57e480bf0a)

#### Kovan explorer problem
----
When you swap on Kovan testnet and click on "view explorer" it will not point you to the actual transaction but to the "Txnhash not found" on the Ropsten testnet explorer.
<br />

[Screenshot Ropsten explorer](https://github.com/JordyDutch/images/blob/main/Ropsten%20explorer%20link-kovan.png?raw=true)

- In console this appeared when clicking on view transaction

```Fired outbound link event kovan.etherscan.io/tx/***```

[Browser Console](https://github.com/JordyDutch/images/blob/main/Console%20warnings%20transcations.png?raw=true)


##### warnings that appear in console for depreicated packages
- event 'close' is deprecated use 'disconnect'
- event 'networkChanged' is deprecated use 'chainChanged'
- 'ethereum.send() is deprecated use 'ethereum.sendAsync()'

[Browser Console transaction](https://github.com/JordyDutch/images/blob/main/Console%20warnings%20website.png?raw=true)

## Suggestions for features

#### Copy adress with a `click`
----
Add the feature to copy your wallet adress in the right top. It already looks like you can click on it to copy it but it doesn't work. We didn't think it is a bug but probably a feauture what isn't added yet.


[Screenshot adress copy](https://github.com/JordyDutch/images/blob/7511834ace5622d21c9f7ff28659042b9ab6ed06/Click%20to%20copy%20adress.png?raw=true)

#### Disconnect wallet from website
---
Add a feature what shows which network is active while you are using the swapper. Probably it would look nice next to the button where you can copy your adress `Screenshot adress copy.`

## Summary
----
Overall the swapper looks very smooth, the transcations are executing fast. We only found a few minor bugs and listed them above.
