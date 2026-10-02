# KotoType v0.9.12 試験版

更新日: 2026-10-03

Windows 11 x64 向けの試験版です。Windows 10 は対象外です。

## この版で直したこと

- 通常の音声入力ショートカットでも、文章の整え方が「この PC」または Gemini のときは整形後の文を貼り付けます。
- 「整形しない」を選んだ場合だけ、生の文字起こしを貼り付けます。

## 配布ファイル

`KotoType_0.9.12_x64-setup.exe`

SHA-256:
`d23cef98b6e2ddf9f385427f7d80a109c2fbeb1f774a904eb852fe7ee1bf09be`

[SHA256SUMS.txt](https://github.com/pandamarumarke-code/kototype-releases/releases/download/v0.9.12/SHA256SUMS.txt)

PowerShell で確認する場合:

```powershell
Get-FileHash .\KotoType_0.9.12_x64-setup.exe -Algorithm SHA256
```

## 既知の条件

- Gemini を使うには、Google ログインとは別に Google AI Studio の Gemini API キー登録が必要です。
- USB マイクの長時間入力、CER 8% 基準、NEC LAVIE は未検証です。
- 初回起動時に SmartScreen が表示される場合があります。