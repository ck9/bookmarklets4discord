## About
Discordの各種サイト共有用ブックマークレット

## Usage

### Amazon.co.jp
amazon.co.jpの商品ページで実行すると、ASIN情報コードのみのシンプルなURLをクリップボードにコピーします。
```javascript
javascript:(()=>{navigator.clipboard.writeText(`https://www.amazon.co.jp/dp/${document.getElementById('ASIN').value}`).then(e => console.error(e));})();
```

### twitter.com (x.com)
twitter.com(x.com)の個別ツイートページで実行すると、Discord上でOGP(ユーザー名,ツイート本文,添付画像など)が展開表示可能なURLに置換してクリップボードにコピーします。  
Thanks: [dylanpdx/BetterTwitFix](https://github.com/dylanpdx/BetterTwitFix)
```javascript
javascript:(()=>{navigator.clipboard.writeText(`https://vxtwitter.com${location.pathname}`).then(e => console.error(e));})();
```
