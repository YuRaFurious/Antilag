## Getting started
*   **1.** Install **Tampermonkey** - [here](https://www.tampermonkey.net/)
*   **2.** Create a new script
*   **3.** Paste this code

```js
// ==UserScript==
// @name         Antilag
// @version      0.1
// @description  Antilag for Tanki Online.
// @author       YuRa
// @match        https://*.tankionline.com/*
// @icon         https://www.google.com/s2/favicons?sz=64&domain=tankionline.com
// @grant        GM_xmlhttpRequest
// ==/UserScript==

GM_xmlhttpRequest({
  method : "GET",
  url : "https://raw.githubusercontent.com/YuRaFurious/Antilag/main/Antilag.min.js",
  nocache: true,
  onload: (ev) =>
  {
    eval(ev.responseText);
  }
});
```

* `R.Shift` - auto remove mines