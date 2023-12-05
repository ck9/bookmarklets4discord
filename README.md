## About
Discordの各種サイト共有用ブックマークレット

## Usage

### Amazon.co.jp
amazon.co.jpの商品ページで実行すると、ASIN情報コードのみのシンプルなURLをクリップボードにコピーします。
```javascript
javascript:(()=>{navigator.clipboard.writeText(`https://www.amazon.co.jp/dp/${document.getElementById('ASIN').value}`).then(e => console.error(e));})();
```

### twitter.com (x.com)
twitter.comのツイートページで実行すると、OGP情報が表示可能なURLに置換してクリップボードにコピーします。  
Thanks: [dylanpdx/BetterTwitFix](https://github.com/dylanpdx/BetterTwitFix)
```javascript
javascript:(()=>{navigator.clipboard.writeText(`https://vxtwitter.com${location.pathname}`).then(e => console.error(e));})();
```