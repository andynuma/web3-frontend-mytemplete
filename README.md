# truffleでの確認コマンド

~~~
truffle(development)> const sender = web3.eth.accounts[1]
undefined
truffle(development)> const balance = web3.eth.getBalance(sender)
undefined
truffle(development)> web3.fromWei(balance,"ether")
BigNumber { s: 1, e: 2, c: [ 100 ] }
truffle(development)> const receiver ="0x32Ce910EbB3ffCaBFc050F7103906B302d3a958B"
undefined
truffle(development)> const amount = web3.toWei(90,"ether")
undefined
truffle(development)> web3.eth.sendTransaction({from:sender,to:receiver,value:amount})
'0xdb99bc10e8e8da90ec147f3b7f507ab8c25665f2b9f670c92a1f656f10a126b6'
~~~
