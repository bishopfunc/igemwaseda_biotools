# Data Visualization Tool
## インストール
- Step1: https://github.com/bishopfunc/igemwaseda_biotools/releases/tag/v1.0.1 からzipファイルをダウンロードし解凍する。
- Step2: `main.app` または `main.exe`を実行

- `.exe`, `.app`, `.zip`の拡張子はコンピューターにウィルスと認識される可能性があります。コンピューターにブロックされた際に以下の手順に従ってください。
  - Mac: https://support.apple.com/ja-jp/HT202491
  - Windows: https://www.buffalo.jp/support/faq/detail/124145337.html
- また、情報セキュリティ上のリスクを軽減するため、**研究室等のコンピューターにこのアプリを絶対にダウンロードしないで下さい**。


## チュートリアル
- Step1: 実験データファイルを開く。日付を入力する。
- Setp2: well情報とその数をサンプルに従い書き換える。
- Step3: `Table`,`Show` などのボタンでデータの表形式及びグラフが正しいか確認する。(`Table1`, `ShowMerge`などについても同様である。)
- Step4: `Save`ボタンをクリックし、グラフの保存先とファイル名を指定し保存する。

sample動画: https://drive.google.com/file/d/1BGkjgN61BzuDIIUZysG7YS29scEHmp6s/view?usp=sharing

## テスト用データ
- 実験データ
	- [220209_AtzR_segment1.txt](https://github.com/bishopfunc/igemwaseda_biotools/files/8192236/220209_AtzR_segment1.txt)
	- [220209_AtzR_segment2.txt](https://github.com/bishopfunc/igemwaseda_biotools/files/8192237/220209_AtzR_segment2.txt)

- well情報

	|サンプル|well情報|
	|----|----|
	AtzR-enriched	|D3
	AtzR-enriched	|D4
	N -CYA		|D5
	N -plasmid	|D6
	AtzR plasmid 	|D7
	AtzR plasmid 	|D8
	N -CYA		|D9
	N -plasmid	|D10

- 結果
	- ![220209_result](https://user-images.githubusercontent.com/61902652/156916552-1499915d-8820-467c-a258-70dd0d9196ef.png)


## Modeについて
- `1 seg mode`と`2 seg mode`の二種類を上のタブで切り替えることができる。
- `1 seg mode`はグラフ化したい実験データのファイルが1つのときに使用する。
- `2 seg mode`はグラフ化したい実験データのファイルが2つのとき、両者を結合したグラフを出力できる。

## ボタンについて
### 1 seg mode
- `Table`: データを表示する。
- `Plot`: グラフを表示する。
- `Save`: グラフの保存先とファイル名を入力し、保存する。
### 2 seg mode
- `Table1`: ファイル1のデータを表示する。
- `Plot1`: ファイル1のデータをグラフで表示する。
- `Table1`: ファイル2のデータを表示する。
- `Plot2`: ファイル1のデータをグラフで表示する。
- `TableMerge`: 結合したデータを表示する。
- `PlotMerge`: 結合したデータをグラフで表示する。
- `Save`: **結合したデータ**のグラフの保存先とファイル名を入力し、保存する。

## 警告について
入力情報が不足している場合、以下の警告(popup)が起こるよう定義しています。

- `ファイルが入力されていません!`
- `ファイルの種類が間違っています! *.txtファイルを開いて下さい!`
- `日付が入力されていません！`
- `Well情報のフォーマットが間違っています行末に余計な(,)がないか、("")と({})が抜けてないか確認しましょう!`
- `データ列数とwell数の合計が一致しません！もしくはwellの情報が重複しています！`
- `ファイルの種類が間違っています! *.pngファイルで保存して下さい!`

## ショートカット
- well情報の入力フィールドは、以下の一般的なショートカットには対応しています！

|  意味  |  Windows  |  Mac  |
|  ----  | ---- | ---- |
|  コピー   |  `ctrl + C`  |  `command + C`	  |
|  貼り付け |  `ctrl + V`  |  `command + V`  |
|  切り取り |  `ctrl + X`  |  `command + X`  |
|  undo     |  `ctrl + Z`  |  `command + Z`  |
|  redo     |  `ctrl + Y`  |  `command + shift + Z	`  |
	

## 確認済みのバグ
- `Plot`ボタンをクリックし画像を表示させたあと、グラフが別画面で立ちあがる。MacOSの場合、その画面を拡大するとアプリがクラッシュする。

## 参考
- グラフ作成の部分は須賀さんのテンプレートを利用させて頂きました 🙇‍♂️
	- https://waseda.app.box.com/file/897161649933
	- https://waseda.app.box.com/file/899039605959

## Google Form
- バグの報告、使用方法の質問、追加機能の要望等があればこちらにご連絡ください。https://forms.gle/JgmBRNZM6xCwacoMA

