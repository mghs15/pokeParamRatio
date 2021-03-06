# pokeParamRatio
ポケモンの隠しパラメータの貢献度を可視化したい

https://mghs15.github.io/pokeParamRatio/

## 概要
ポケモンの隠しパラメータ等（ファン用語で種族値・個体値・努力値）が実際の数値に対してどの程度貢献しているのか可視化する簡易ツール。
以下の部分を目的のデータに変換する（以下の例は、しんちょうレジギガスのHD極振りあまりB）。
```
  const shuzokuVal = [110,160,110,80,110,100]; //種族値：ポケモンの種類ごとに固定
  const kotaiVal = [31,31,31,31,31,31]; //個体値：個体ごとに変化
  const doryokuVal = [252,0,4,0,252,0]; //努力値：個体ごとに変化
  const seikakuHosei = [1.0,1.0,1.0,0.9,1.1,1.0]; //性格補正：個体ごとに変化
  const targetLv = 50; //レベル：50で固定
```


## 注意点・参考文献等
* 「[ポケットモンスター　ソード・シールド](https://www.pokemon.co.jp/ex/sword_shield/)」というゲーム作品で遊ぶための補助ツールです。使われている用語等含めて非公式なものです。
* ポケットモンスター・ポケモン・Pokémonは任天堂・クリーチャーズ・ゲームフリークの登録商標です。
* 数値や計算方法はポケモンWiki（ https://wiki.ポケモン.com/wiki/ ）を参照。
* グラフは[Chart.js](https://www.chartjs.org/)を利用。
