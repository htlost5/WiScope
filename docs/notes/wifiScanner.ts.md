---
id: n3031z1yuf88qienw8kv3cp
title: ts
desc: ""
updated: 1769584608736
created: 1769583980551
---

## wifiScannerのロジックに関して

### 目的

- android APPに周囲のアクセスポイントをリサーチさせ、BSSID、信号強弱を取得し、リスト化すること
- 主にネイティブモジュールを構築することを目的とする
- 最終目標は、アプリ側でのAPリストを表示

### nativem module の構築に関して

#### 必要情報

- BSSID
- 信号強弱

#### ロジック構想

1. 周囲のAPを分析
2. BSSIDと信号の強弱をセットにしてあるだけ取得
3. 取得した全データをリスト化
4. そのままreactnative側へreturn
