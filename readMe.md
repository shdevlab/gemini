gemini API module
==========
> Google's generative api Used module

 > # Info
 >
 > Used Dir : ```< root.Dir > /gemini/```
 >
 > Current Vir : betav1
 >
 > current MimeType : ```image/png```

 > # How to Check available Api KEY?
 >
 > This module gets gemini api model list for check availd models
 >
 > This needs availd gemini api key
 >
 > So, it check api key in this process !
 
 > # Example
 >
 > < !-- In msgbotR -- >
 ```js
let gemini = require("gemini-module");
gemini.create({
  "model": "gemini-1.5-flash-latest",
  "apiKey": "WRITE_YOUR_API_KEY"
});

let response = gemini.getResponse({
  "type": 0, // 0 or 1 { 0 : text, 1 : addictional }
  "prompt": {
     "text": "안녕"
  }
});

Log.info(response);
```