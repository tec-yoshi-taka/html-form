# HTMLのformについて

## スライド資料
<br>

---

## form要素について
入力エリア全体をform要素で囲う
-actionにはデータ送信先URL
-methodには送信方法（通常はpost）
を設定

```html
<form action="test" method="post">
```
<br>

## dl/dt/dd 要素について
### 定義リストはdlタグで範囲で表し、
### 定義する用語dtタグで
### 用語の説明をddタグで表します。

```html
<dl>
	<dt>用語</dt>
	<dd>用語に対する説明</dd>
</dl>
```
<br>

<br>

# 入力用部品 input
### type="text" は文字列を入力
### name属性はデータを入れる入れ物の名前を指定 
```html
<dl>
    <dt>お名前:</dt>
    <dd><input type="text" name="name"></dd>
</dl>
```
<br>

### メールアドレスの場合はスマホ用キーボードの設定inputmode属性を指定 
```html
<dl>
	<dt>メールアドレス:</dt>
	<dd><input type="text" inputmode="email" name="email"></dd>
</dl>
```
<br>


---

# 選択用部品 select option
### 多数の項目の中から選択する場合、
### 全体をoption要素で囲み、name属性を設定する
### 各項目をselect要素で設定し、送信データをvalue属性で設定する

```html
<dt>年齢:</dt>
<dd>
    <select name="age">
        <option value="0">選択してください</option>
        <option value="10">10代</option>
        <option value="20">20代</option>
        <option value="30">30代</option>
        <option value="40">40代</option>
        <option value="50">50代</option>
    </select>
</dd>
```
<br>

# 一つのみを選択する部品 input type="radio"
### name属性の値でグループ化し、選択できる項目は一つ
### value属性で送信データを指定
### 文字とinput要素を<label>～</label>で囲む

```html
<dt>性別:</dt>
<dd>
	<label><input name="gender" type="radio" value="男" checked>男</label>
	<label><input name="gender" type="radio" value="女">女</label>
	<label><input name="gender" type="radio" value="その他">その他</label>
</dd>
```
<br>


# 複数を選択する部品 input type="checkbox"
### name属性の値でグループ化し、選択できる項目は複数
### value属性で送信データを指定
### 文字とinput要素を<label>～</label>で囲む

```html
<dt>趣味:</dt>
<dd>
	<label><input name="hobby" type="checkbox" value="スポーツ">スポーツ</label>
	<label><input name="hobby" type="checkbox" value="読書">読書</label>
	<label><input name="hobby" type="checkbox" value="ショッピング">ショッピング</label>
</dd>
```
<br>

---

# ランダムでPCのじゃんけんの手を決める
## 以下の作業をjanken.pyでおこなってください

-下記のPC用画像ファイル名をリストに入れる
    -'gu_female.png', 'choki_female.png', 'pa_female.png'

-ランダムで0，1，2の数字を生成する

-じゃんけんアルゴリズムをつかって、ユーザの手とPCの手で勝敗を確認してください
    -勝敗の結果を 変数 data に格納してください
        -ユーザが勝った場合 → あなたの勝ち
        -ユーザが負けた場合 → あなたの負け
        -あいこの場合 → あいこ




