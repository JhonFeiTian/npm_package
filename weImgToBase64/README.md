## weImgToBase64

[中文](https://github.com/ougege/npm_package/blob/master/weImgToBase64/README-CN.md '中文')

#### install
```SHELL
npm install weimgtobase64
# common JS
const weimgtobase64 = require('weimgtobase64')
# es6
import weimgtobase64 from 'weimgtobase64'
```

#### use
```JS
// parse img url
let url = 'http://img.qipeiren.com/UploadFile/UserProPic/2019/11/23/4b65b8aadcfb0ac65a91.jpg'
console.log(weimgtobase64.parse(url))
// parse img object
let img = document.getElementById('test')
console.log(weimgtobase64.parse(img))
// useCanvas img object
let img = document.getElementById('test')
console.log(weimgtobase64.useCanvas(img))
```

#### function

function|parameter|default|required|description|
--|--|--|--|--|
parse|string/object||optional|a img object or img url|
useCanvas|object||required|a img object|


#### tips
As soon as you draw into a canvas any data that was loaded from another origin without CORS approval, the canvas becomes tainted.A tainted canvas is one which is no longer considered secure, and any attempts to retrieve image data back from the canvas will cause an exception to be thrown.

#### wiki
1. [Allowing cross-origin use of images and canvas](https://developer.mozilla.org/en-US/docs/Web/HTML/CORS_enabled_image 'Allowing cross-origin use of images and canvas')