# Brawl Stars API Proxy
This repository is an edited version of [brawlstars](https://www.npmjs.com/package/brawlstars) javascript wrapper.

## What & Why was this made?
- This is an unofficial wrapper of the official brawl stars API with proxy.
Many developers don't/can't use brawl stars API due to the fact that it is IP bounded. But this solves their problem.

- The proxy used here is provided by [royaleapi.com](https://royaleapi.com/).
 You can read the documentation [here](https://docs.royaleapi.com/#/proxy).

## How to use?

#### 1. Refer the [usage](https://www.npmjs.com/package/brawlstars#usage) page of [brawlstars wrapper](https://www.npmjs.com/package/brawlstars) for more info.

##### Example Usage:
Simply import the `Client` class and instantiate it with your API token:
```js
// TypeScript, ESM

import  {  Client  }  from  "brawlstars";

// CommonJS, Node.js

const  {  Client  }  =  require("brawlstars");

// Create instance

const  client  =  new  Client("TOKEN",  { 

 cache:  true,  // default is true

 cacheOptions:  undefined  /* options for node-cache, default is undefined. */

});

// Call into functions

client.getPlayer("TAG")

 .then((player)  =>  console.log(player.name))

 .catch((err)  =>  console.error(err));
```

#### 2. Obtaining API Token & Whitelist IP
You can create an API Token on the official [brawl stars developer website](https://developer.brawlstars.com/#/getting-started).

While creating a "API Token" you will be asked to whitelist IPs, here just simply whitelist`128.128.128.128` IP address:

![IP Whitelist](https://iili.io/fAdhOu.png)

#### 3. Last small thing
Click on "Create Key" and you will get your access token.
Now just replace the TOKEN with your access token.

*Note: You should always keep your token private.*
With this you would be able to connect with the API from any IP Address.

## Useful Links

 - [Brawl Stars Developer Portal](https://developer.brawlstars.com/#/getting-started)
 - [brawlstars API Wrapper](https://www.npmjs.com/package/brawlstars)
- [Royale API Proxy Docs](https://docs.royaleapi.com/#/proxy)
