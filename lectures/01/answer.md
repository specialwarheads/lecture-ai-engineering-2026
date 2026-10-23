# 第1回 解答

## 演習

- 講座に固有の質問（宿題の3レベル）へのモデルの回答（要約でよい）： 一般的な内容で回答した。
- 用語集の正しい意味と比べて気づいたこと： 基礎/応用/発展という3段階であることは抽象的には推測できているが、基礎/実装/発展という本講座の特有な定義には対応できていない。
- 表示できたトークン数（入力 / 出力）： [tokens] input=22, output=432

## 宿題

- 取り組んだレベル： 基礎 / 発展
- やったこと： ask.pyを入出力トークン数と応答時間を出力するように変更し、4種のモデルで実行して結果を比較した。
- 結果：
[model] gemini-3.5-flash-lite
[tokens] input=7, output=625
[time] response=2.72s

[model] gemini-3.5-flash
[tokens] input=7, output=625
[time] response=10.20s

[model] gemini-3.6-flash
[tokens] input=7, output=566
[time] response=10.89s

[model] gemini-3.8-flash
[tokens] input=7, output=769
[time] response=171.13s
- 気づき・疑問： 
モデルによって出力内容およびトークンが変化し、特にgemini-3.8-flashの応答時間が非常に長い(約3分程度)ということが分かった。
逆に応答時間が最も短いのが軽量のgemini-3.5-flash-liteモデルであった。