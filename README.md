# TinyHSP

TinyHSPは**最軽量のHSPを作成する**ことを目標にしたプロジェクトです。マルチプラットフォーム（Windows・Linux・macOS）で動作する**TinyHSPコンパイラとエンジン**を作成することを目指しています。

## TinyHSPの仕様（暫定案）

Palo Alto Tiny BASICを参考にした仕様になっています。

- プリプロセッサ
    - なし
- 命令
    - pset
    - color
    - redraw（引数はなし。redraw 1に相当）
    - title
- 関数
    - rnd（randomize使用時に相当）
- 構文
    - 繰り返し: repeat...loop（カウンタ変数cntはなし）
    - ジャンプ: \*ラベル・goto・gosub・return
    - 条件分岐: if 比較式 : 処理（else文はなし）
- 変数
    - 変数はa-zの26個のみ
    - 配列は@のみ（一次元配列）
- コメント
    - ;（行頭のみ）
- システム変数
    - システム変数key（stick key,1+2+4+8...相当のキー情報が代入される）
- 演算子
    - 比較演算子: ==, !=, >, >=, <, <=
    - 算術演算子: +, -, *, /

## コミッターさん向けのガイド

このプロジェクトは__楽しんで開発しよう__という基本方針で動いています。コミッター向けのルールは次のようなものです。

1. 開発すること自体を楽しむ
2. コミットメッセージは自由に書く
3. C言語で実装する
4. GUIはOpenGL+GLFWで実装する

詳しくはWikiのページ[プロジェクトのルール](https://github.com/dolphilia/tinyhsp/wiki/プロジェクトのルール)をご覧ください。

## どんなことでもissuesにどうぞ

Githubでは掲示板のスレッドのような機能「イシュー」を使うことができます。質問や提案がありましたら、ご自由に[Issuesのページ](https://github.com/dolphilia/tinyhsp/issues)からイシューを立てていただければと思います。

※ 注意すべき点として、イシューは削除することができません。イシューを立てる際には内容をよく吟味するようお勧めします。

## リンク

- きっかけ: [TinyHSPの提案](http://hsp.tv/play/pforum.php?mode=all&num=77515)

## ライセンス

TinyHSPはMITライセンスです。
