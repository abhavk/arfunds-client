# arfunds-client

This repository demonstrates usage of the `arfunds` npm package. Sample code is available in `index.html`. 

Install arfunds

In order to run this in your own web package, copy the `bundle.js` to your own repository and import it using:
```
<script src="bundle.js"></script>
```

Fetch all Arfund contract IDs
```
var contracts = await getAllContracts();
```

Interact with a particular Arfund contract
```
var fund = new Arfund(contractId, arweave, true);
var state = await fund.getState(state);
```

Contribute an `amount` to an Arfund contract
```
var interaction = await fund.contribute(amount);
```

Use `arfunds` on your server:

```
npm install
```

Run a sample server (requires ArConnect wallet)
```
npm serve
```  
