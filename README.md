# node-imageinfo

An SWF only fork of [NorgannasAddOns/node-imageinfo](https://github.com/NorgannasAddOns/node-imageinfo). The original node-imageinfo wouldn't work for me, due to updates to zlib and issues with the original code. So I fixed it, but I only need it for SWF files.

## Usage:
Clone this repository into node_modules/imageinfo.
```javascript
var imageinfo = require('imageinfo'),
    fs        = require('fs');

fs.readFile('test.swf', function(err, data) {
	if(err) throw err;
	imageinfo(data, function(info) {
		console.log(info);
	});
});
```

## License:
Still CC0.