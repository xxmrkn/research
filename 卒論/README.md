# 本フォーマットについて
これは [東京大学工学部計数工学科  |  LaTeXテンプレート](https://www.keisu.t.u-tokyo.ac.jp/research/latex/) を基に一部修正を加えたものになります．

基本的には上記サイトにある情報や本パッケージ付属の suribt.pdf を参照してください．

コンパイルには `platex + dvipdfmx` を前提としています．

# 修士論文の設定
`\documentclass[master, ...]` のように `documentclass` のオプションとして `master` を指定してください．

# 便利なコマンド
図や表，数式を参照する際に便利なコマンドをプリアンブルで定義しています．

```tex
\newcommand{\fref}[1]{図\ref{#1}}
\newcommand{\tref}[1]{表\ref{#1}}
\newcommand{\eref}[1]{式\eqref{#1}}
```

例えば，`図1` のように表示する場合， `図\ref{label}` のようにしていたところを `\fref{label}` のようにします．

数式については，括弧つきの式番号 `式(1.1)` のようになります．
