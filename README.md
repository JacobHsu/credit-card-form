# credit-card-form

A fantastic credit card form with smooth and sweet micro-interactions. Includes number formatting, validation and automatic card type detection. Built with vuejs and also fully responsive.

See Live: https://codepen.io/JavaScriptJunkie/pen/YzzNGeR

![](demo.gif)

# references

[Reset CSS](https://meyerweb.com/eric/tools/css/reset/) 重置歸零 – 網頁排版各瀏覽器快速一致化  
[Google Fonts API](https://developers.google.com/fonts/docs/css2)  
[信用卡冷知識―起源、卡別、卡號怎麼來](https://www.money101.com.tw/blog/冷知識-信用卡卡號不是這麼簡單的！)
信用卡開頭數字代表不同的卡片用途： `3：旅遊、娛樂與金融機構(如JCB、美國運通)　 4：Visa` `5：Mastercard`　  

## notes

`{{n < 10 ? '0' + n : n}}`  月份小於10 前補0  

`CVV (Card Verification Value)` 信用卡安全檢查碼  聚焦：focus/blur 聚焦/失去焦点  
`flipCard()` 翻轉卡面  `<div class="card-item" v-bind:class="{ '-active' : isCardFlipped }">`

其他欄位會觸發 methods:  `focusInput (e)`  改變 focusElementStyle css [ransform](https://developer.mozilla.org/zh-TW/docs/Web/CSS/transform)
[CSS animate 水平翻轉](https://codepen.io/Inu/pen/vOKJgd)  

# npm 

[![NPM](https://nodei.co/npm/vue-the-mask.png?downloads=true&stars=true)](https://www.npmjs.com/package/vue-the-mask)[![NPM](https://nodei.co/npm/gh-pages.png?downloads=true&stars=true)](https://www.npmjs.com/package/gh-pages)  

### gh-pages

`$ npm init -y`  
`$ npm install gh-pages --save-dev`  

package.json
```js
  "scripts": {
	...
    "deploy": "gh-pages -d ."
  },
```
`$ npm run deploy`  
https://jacobhsu.github.io/credit-card-form/  
