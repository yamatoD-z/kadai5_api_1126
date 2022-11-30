# 課題　 --
音声認識、翻訳、読み上げ(Web Speech API、DeepL API)

 
## ① 課題内容（どんな作品か）

- 前回想定の、海外から来たばかりで、意思疎通が難しい家政婦が来たという設定で、翻訳ツールを作成。
- APIは上限に達すると使えなくなるだけですが、しばらくしたら、キーを再生成して無効にしておきます（メインＰＣが音声認識しなく、デプロイしたものをラップトップやスマホで挙動確認）
- 

## ② 工夫した点・こだわった点

- Web Speech APIは、句読点がつかない。そのまま翻訳するとしっかり翻訳されないため、句点の追加が必要となった。典型的な句点は、replaceを使用して、追加作業をサポート。
- 音声認識の過程が見えるようにした。
- Web Speech APIの読み上げは、15秒で切れる。ネットで調べても有名な事象の模様。ただ、一時停止＆再開を5秒ごとに行うことで、継続させることが出来た。
- 
- 

## ③ 難しかった点・次回トライしたいこと(又は機能)

- 各パーツはネットから拾ってきたものを調整。ただし、ＤｅｅｐＬＡＰＩは何をしているのか理解出来ないまま。
- 音声認識はやや挙動が不安定。大量に同じ言葉を読み込んで反映することがある
- 実用性という意味では、テンポは悪く、難しいものの、ワンクリックですべての機能を動かせれば。

## ④ 質問・疑問・感想、シェアしたいこと等なんでも

- [質問]
- [疑問]
- [感想]ネットで拾ったものを組み立てられるというのも、それはそれで前進しているんだと思う。
- [tips]
- [参考記事]
音声認識
https://zenn.dev/tomioka/articles/47af891c679ca3
読み上げ
https://www.petitmonte.com/javascript/web-speech-api.html
DeepL
https://qiita.com/redchili/items/337f3c338b12f494766e