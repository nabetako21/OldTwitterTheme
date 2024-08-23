# OldTwitterTheme
[OldTwitter](https://github.com/dimdenGD/OldTwitter/) で個人的に使用しているカスタムCSSを公開します。<br>

## こんなテーマ
* ツイートヘッダー周りの変更
  * フルネームの隣にあったユーザーネームを下に移動
  * ツイート内容をアイコンの下に置き、右側に寄っていたのを横幅いっぱい使って表示
  * 返信元のヘッダーを小さく表示
  * 鍵マークや公式バッチをアイコン右上に配置
  * リツイート者の表示を時刻の下に配置
* 引用リツイートの引用感
  > こういうよくある引用の表現に変更
* タイムラインを圧迫したくないため、1ツイートごとの最大の高さを変更
  * 文字数の多いツイートはスクロールで読めるように変更
  * 画像の表示する高さを狭く変更
  * 詳細画面では通常通り表示
* センシティブな画像をぼかしてチラ見せ
  * センシティブ設定をしている画像をぼかす（クリックで表示可）
  * 詳細画面では通常通り表示
* 背景を変更できるように
  * タイムラインなどを背景を半透過＆ぼかし

## 使用方法
* OldTwitterのカスタムCSSに以下を記述
  ```CSS
  @import url('https://nabetako21.github.io/OldTwitterTheme/Metro-OldTwitter.css');
  ```

## 拡張CSS
カスタムCSSに追記すると楽しい(?)設定<br>
* フォント変更（Google Fonts使用）
  ```CSS
  /* 自分はこれを使用してます */
  @import url('https://fonts.googleapis.com/css2?family=Murecho:wght@450..900&family=M+PLUS+2:wght@450..900&display=swap');
  :root {
    --font: "Murecho","M PLUS 2",sans-serif !important;
    --tweet-font: "Murecho","M PLUS 2",sans-serif !important;
  }
  ```
* 背景の変更
  ```CSS
  body {
    /* 背景画像の設定（デフォルトはTwitterの雲のやつ） */
    --bg: url(画像のリンク);
    /* 好みで var(--background-color) をブレンド */
    background-blend-mode: multiply;
  }
  ```
* 色の変更
  ```CSS
  /* 背景半透過のために OldTwitter での設定を上書きしていますが、
   * 上書き仕返せば一応変更できます */
  body {
    --background-color: #ffffffaa !important;
    --dark-background-color: #f5f8faaa !important;
    --darker-background-color: #f5f8facc !important;
    --border: #66757f33 !important;
  }
  ```
