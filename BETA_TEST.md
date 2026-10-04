# KotoType v0.9.19 試験版配布

Windows 11 x64・Apple Silicon Mac向けの試験版です。Windows 10・Intel Macは対象外です。利用には運営者が承認したGoogleアカウントが必要です。

使い方は[こちら](USER_GUIDE.md)をご覧ください。

## この版で直したこと

- 初回設定と通常設定から、ローカル整形用データ約7.1GBを取得できるようにしました。
- 全4ファイルのSHA-256を検証してから、ローカル整形を使用します。通信断や中断後は再開できます。

## 配布ファイル

- Windows 11: `KotoType_0.9.19_x64-setup.exe`
- MシリーズMac: `KotoType_0.9.19_aarch64.dmg`

[最新版のダウンロード](https://github.com/pandamarumarke-code/kototype-releases/releases/latest) / [SHA-256](SHA256SUMS.txt)

ソースコードのZIPは不要です。上記のインストーラーまたはDMGを使ってください。

## 確認済みの範囲と残件

- Windowsではマイク入力・句読点・改行・録音中の消音と復帰・貼り付けを確認しています。新しい取得処理では、既存モデル7.1GBのSHA検証と公開配布先のRange応答、再開・取消・破損検出のテストを確認しました。
- Mac実機での新規7.1GB取得から整形までの通し確認は未完了です。
- 認識精度のCER 8%目標は未達であり、誤認識や固有名詞の誤りが残る場合があります。重要な文章は送信前に確認してください。
- Gemini を使うには Google AI Studio の Gemini API キー登録が必要です。
- Windows版は未署名、Mac版は未署名・未公証です。初回OS警告の解除と、マイク・Macのアクセシビリティ許可が必要です。
