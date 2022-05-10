# arfunds-client

This repository demonstrates usage of the `arfunds` npm package. Sample code is available in `index.html`. 

Install arfunds

In order to run this in your own web package, copy `arfunds_bundle.js` to your own repository and import it using:
```
<script src="arfunds_bundle.js"></script>
```

Run the `index.html` server (requires ArConnect wallet)
```
serve
```

## Available Methods

Fetch all Arfund contract IDs
```
var contracts = await getAllContracts();
```

Connect with and get the state of a particular Arfund contract
```
var fund = new Arfund(contractId, arweave, true);
var state = await fund.getState(state);
```

Contribute an `amount` to an Arfund contract
```
var interaction = await fund.contribute(amount);
```

## Server Side
Use `arfunds` on your server:

```
npm install --save arfunds
```

Import Arfunds methods
```
import Arfund, { getAllContracts } from "./Arfunds";
```


