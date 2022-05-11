# arfunds-client

This repository demonstrates usage of the [arfunds](https://github.com/abhavk/arfunds) npm package. Sample code is available in `index.html`. 

Install arfunds

In order to run this in your own web app, import it using:
```
<script src="https://unpkg.com/arfunds@latest/umd/arfunds_bundle.js"></script>
```

Run the example `index.html` server (requires ArConnect wallet):
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


