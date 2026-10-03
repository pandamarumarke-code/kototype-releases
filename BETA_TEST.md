# KotoType v0.9.13 試験版配布

公開日: 2026-10-03

Windows 11 x64 向けの試験版です。Windows 10 は対象外です。

## この版で直したこと

- ローカル整形時に「一旦」が「1旦」と扱われて安全ガードにより整形全体が破棄され、句読点が入らなくなる問題を修正しました。文章はローカル整形のまま貼り付けます。
- 初回更新時に「録音中はスピーカーを消音」を有効化します。録音開始で既定の再生デバイスを消音し、終了時に開始前の消音状態へ戻します。設定画面で切り替えられます。

## 配布ファイル

`KotoType_0.9.13_x64-setup.exe`

SHA-256:
`b0ad73c8d051a9dea5f04d0d7b1542e860f7795769a3eb4a40fa981687510133`

[GitHub Releases: v0.9.13](https://github.com/pandamarumarke-code/kototype-releases/releases/tag/v0.9.13)

PowerShell で確認する場合:

```powershell
Get-FileHash .\KotoType_0.9.13_x64-setup.exe -Algorithm SHA256
```

## 未完了の確認

- 実マイクでの長文入力、整形結果、録音中のスピーカー消音と復帰は、利用環境ごとに確認が必要です。
- Gemini を使うには Google AI Studio の Gemini API キー登録が必要です。
- 初回配布時の SmartScreen 表示が出る場合があります。
