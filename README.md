# amazon-asin-scraper

Making your amazon scraping job easier. This is going to be an alternative way to get the data you need that are not available on aws product and mws search api.

 - Only Supports US marketplace as of this moment.

# Installation

```shell
npm install amazon-asin-scraper
```

## Usage

```js
const asinScraper = require('amazon-asin-scraper');

// using callback
let options = {
    asin : someAsinHere,
    proxy : '', //optional
    userAgent : '' //optional
  };

asinScraper(options, (result)=>{
  // result below
  // {
  //   asin :
  //   sellerList : [
  //       {
  //         productTitle :
  //         customerReview :
  //         sellerName :
  //         sellerRating :
  //         fulfulledBy :
  //         primeBadge :
  //         offerPrice :
  //         shipping :
  //         merchantID :
  //         offerListingId :
  //       },
  //       {},
  //       {}
  //   ]
  // }  
});
```

## Features

- Buybox Page Data Scraping
- Review Scraping
- Full Seller List Detail
- Product Detail Page Data Scraping
- Single proxy or multiple proxies and handles proxy failure
- Cookie jar and custom cookies/headers/user agent
- Set Retries on failed requests

## Documentation

For documentation and examples check out [https://not-yet.com](https://cjpcjp.jd)
