<img width="1926" alt="Screenshot 2024-01-10 at 5 33 24" src="https://github.com/MoomA-0750/horizontal-comments-css/assets/23278754/6d33c1d3-d8db-436e-9a5f-aed5df9eccb7">

おそらく結構荒削り状態だと思われるので、何か見つかった際は、issueを建てていただくか、Xアカウントにでも連絡下さいますと助かります

とりあえずこのレポジトリにあるCSSファイルの中身を丸コピして、OBSのカスタムCSS欄に貼り付けていただければ動くはずです

### カスタムの仕方
cssファイルのトップにある以下の部分で、基本的なカスタムはできるようになっています
```horizontal-comments.css
:root {
    /* ユーザーネームの文字色 */
    --username-color: rgba(255, 255, 255, 0.7);
    /* メンバー加入ユーザーの文字色 */
    --membership-user-color: #FFCDE5;
    /* チャット本文の文字色 */
    --message-color: #fff;
    /* 本文アウトライン色 (4個目の数字を0にして無効化) */
    --message-outline-color: rgba(0,0,0,0.35);
    /* 本文文字サイズ */
    --font-size: 20px;
    /* 本文列高さ */
    --line-height: 24px;
    /* フォント */
    --font: "LINE Seed JP_OTF";
    /*コメントと名前の空間*/
    --space: 4px;
    /* コメント間の空間 */
    --gap: 50px;
    /*底の高さ*/
    --floor: 10px;
  }
```

基本的には「:」この記号の後の文字列を変更することにより変更できます

またその際、一番最後にある「;」の記号は残すようにしてください

## 例
### 変更前
```css
/* フォント */
--font: "LINE Seed JP_OTF";
```

### 変更後
```css
/* フォント */
--font: "IBM Plex Sans JP";
```

## 色の指定

記法がわかる場合はそのまま変更していただけますが、わからない場合は下記のツールの使用をお勧めします
（インストールしている場合はPowerToysのColor Pickerも便利かも）

[Color Picker](https://redketchup.io/color-picker)

[色の指定方法](https://so-zou.jp/web-app/tech/css/specification/syntax/color.htm#:~:text=%E9%96%A2%E6%95%B0%E8%A8%98%E6%B3%95%20rgb%20%28red%2C%20green%2C%20blue%29%2016%E9%80%B2%E8%A8%98%E6%B3%95%20%23%20RRGGBB,%2A%2F%20color%3A%20%23f03%3B%20color%3A%20%23ff0033%3B%20%2F%2A%206%E6%96%87%E5%AD%97%E8%A8%98%E6%B3%95%20%2A%2F)

## フォントの指定
一番上の:rootの中の以下の部分を変更してください
```css
/* フォント */
--font: "LINE Seed JP_OTF";
```

## フォント名の確認方法

### Windows
設定アプリに行き、「個人用設定」から「フォント」へ行くと、インストールされているフォントが表示されます

<img width="508" alt="Screenshot 2024-01-10 202427" src="https://github.com/MoomA-0750/horizontal-comments-css/assets/23278754/a56b2aac-c2b8-4752-b018-169fd2376d80">
<img width="930" alt="Screenshot 2024-01-10 202937" src="https://github.com/MoomA-0750/horizontal-comments-css/assets/23278754/2504cf9e-221a-4323-b987-f9726a292216">

使用したいフォントを検索すると結果が表示されるので、目的のフォントの名前をそのまま入力します

<img width="252" alt="Screenshot 2024-01-10 210629" src="https://github.com/MoomA-0750/horizontal-comments-css/assets/23278754/47a146b1-ee9b-4091-9ba5-9935129b1089">

この場合は「IBM Plex Sans JP」がその名前になり、
```css
/* フォント */
--font: "IBM Plex Sans JP";
```
のようになります

### macOS
Font Bookを開き、検索バーで目的のフォントを検索します

<img width="1256" alt="Screenshot 2024-01-10 at 22 19 27" src="https://github.com/MoomA-0750/horizontal-comments-css/assets/23278754/40033a37-f140-4188-9786-ddcaf1f5730e">
<img width="436" alt="Screenshot 2024-01-10 at 22 19 57" src="https://github.com/MoomA-0750/horizontal-comments-css/assets/23278754/947b5ab0-9d16-42b7-93ca-b25bfe46dfea">

結果が表示されるので、目的のフォントの名前をそのまま入力します

<img width="146" alt="Screenshot 2024-01-10 at 22 23 00" src="https://github.com/MoomA-0750/horizontal-comments-css/assets/23278754/f172bbb5-a989-45d6-af2f-f4cda1c90d4b">
<img width="1135" alt="Screenshot 2024-01-10 at 22 22 42" src="https://github.com/MoomA-0750/horizontal-comments-css/assets/23278754/a49f1e0e-271b-4122-9489-c0fd1293d027">


この場合は「IBM Plex Sans JP」がその名前になり、
```css
/* フォント */
--font: "IBM Plex Sans JP";
```
のようになります
