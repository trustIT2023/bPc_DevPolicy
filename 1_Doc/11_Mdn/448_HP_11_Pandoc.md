# マークダウンからHTMLへの変換作業

## 結論

> [!IMPORTANT]  
> **PandocというOSSのソフトを利用します**
> **HTMLに変換することでホームページに、docxに変換することでwordの校閲機能の利用などが可能です。**

## Pandoc

### 環境構築

- [Pandocのインストール](https://docs.zettlr.com/ja/installing-pandoc/)

### マニュアル

- [PandocUsersGuide日本語版](https://pandoc-doc-ja.readthedocs.io/ja/latest/users-guide.html)

### マークダウンからHTMLにCSSを指定して変換する方法

- [pandocでMarkdown形式をHTML/CSSに一発変換(https://qiita.com/fk_2000/items/d9ba2984349728bb5609)
  - pandoc -c style.css input.md -o output.html

### コマンド

#### コマンド実行の参考情報

- [JavaScriptを用いた変換1](https://jsprimer.net/use-case/nodecli/md-to-html/)

#### 適用コマンド

pandoc ./1_Doc/11_Mdn/401_DevPolicy.md -s --embed-resources --standalone  -t html5 -c ./3_Dat/41_Mdn/MkdnTrust.css -o ./3_Dat/42_MdToHtml/401_DevPolicy.html

## 参考情報

### 参考コマンド

pandoc -o 401_DevPolicy.html 401_DevPolicy.md
pandoc -s -o 401_DevPolicyV2.html 401_DevPolicy.md
pandoc -c MkdnTrust.css MkdnTrust.css 401_DevPolicy.md -o 401_DevPolicyV4.html
pandoc -s -o --data-dir="C:\aIT\1_Doc\11_Mdn" 401_DevPolicyV3.html 401_DevPolicy.md

### 参考CSS

```css
handleScroll(e) {
    return e.target.offset.top / e.target.innerHeight;
}

shouldScroll(percentage) {
    var target = React.findDOMNode(this.refs.previewer);
    target.scrollTop = target.innerHeight * percentage;
}
```

### 他の方法（VS Codeから実行する方法)

- [VSCodeでMarkdownをHTMLに変換する](https://qiita.com/youichi_io/items/cee2401a26e742fb447a)
- [VSCodeでmdtodocx](https://it-afi.com/vscode/vscode%E3%81%A7md-to-docx-%EF%BC%88markdown%E3%82%92word%E3%81%B8%E5%A4%89%E6%8F%9B%EF%BC%89%E3%81%99%E3%82%8B%E3%81%AB%E3%81%AFpandoc%E3%83%97%E3%83%A9%E3%82%B0%E3%82%A4%E3%83%B3%E3%82%84/)

#### HTMLに変換できるサイト

- [ConvertMarkdowntoHTML](https://markdowntohtml.com/)

#### その他のHTML変換方法

- [JavaScriptを用いた変換1](https://jsprimer.net/use-case/nodecli/md-to-html/)

## Pandocを用いたトラストのソリューション

### インストーラー

Datファイル配下に格納

### コマンド実行

- エクセルの関数を用いてコマンド一覧の一括実行が可能

### 必要な前準備

- 拡張子をmd→htmlに変換が必要
  - [!Note]などの変換対応
