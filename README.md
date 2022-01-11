# HTMLのformについて

## スライド資料

https://drive.google.com/file/d/1gGgRhzRsK78bqueVOVc6LF_OoShE-fRr/view?usp=sharing

<br>

---

## form要素について
入力エリア全体をform要素で囲う

- actionにはデータ送信先URL

- methodには送信方法（通常はpost）

を設定

```html
<form action="test" method="post">
```
<br>

---

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

---

# 一行のテキストを入力する部品 input
### type="text" は一行の文字列を入力
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

---

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

---

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

# 複数行のテキストを入力する部品 textarea
## rows属性で行数，cols属性で列数を指定できる

```html
<dt>お問い合わせ:</dt>
<dd>
	<textarea name="comments" cols="30" rows="10"></textarea>
</dd>
```
<br>

---

# データ送信用の部品 input type="checkbox"
## value属性で値を表示内容を指定
## ユーザがクリックする場所なので「送信」のように曖昧な表現はしないようにすること


```html
<p>
	<input type="submit" name="submit" value="お問い合せをする">
</p>
```
<br>

---





