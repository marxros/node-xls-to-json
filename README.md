# node-xls-json

Converting xls file to json files using nodejs. Returning the original values from the spreadsheet.

## Install

```
  npm install xls-to-json-3
```

## Usage

``` javascript
  node_xj = require("xls-to-json");
  node_xj({
    input: "sample.xls",  // input xls
    output: "output.json", // output json
    sheet: "sheetname",  // specific sheetname
    rowsToSkip: 5 // number of rows to skip at the top of the sheet; defaults to 0
  }, function(err, result) {
    if(err) {
      console.error(err);
    } else {
      console.log(result);
    }
  });
```

In config object, you have to enter an input path. But If you don't want to output any file you can set to `null`.

Original Package: https://github.com/rodrigograca31/node-xls-to-json

## License

MIT [@chilijung](http://github.com/chilijung)

