# 配布モデルと検証値

インストーラーには音声区間を検出する Silero VAD モデルが含まれます。文字起こしの標準認識モデルと、方式 A に使う整形モデルは別途取得します。出典と検証値は次のとおりです。

## 標準認識モデル

- ファイル: `whisper-large-v3-turbo-Q8_0.gguf`（886,381,760 bytes）
- SHA-256: `b2e30cc286bc9f3aba4db9099fc7403543497c05ce7100d0d83091ddfd25a183`
- 出典: [handy-computer/whisper-large-v3-turbo-gguf](https://huggingface.co/handy-computer/whisper-large-v3-turbo-gguf)、固定リビジョン `5eaf945c7978e564bae5b28a5b1639dd93c2bfb1`
- ライセンス: Apache License 2.0。配布元の [モデルカード](https://huggingface.co/handy-computer/whisper-large-v3-turbo-gguf) は元モデルから継承した Apache 2.0 と明記しています（2026-09-30 確認）。
- 配布タグ: `models-whisper-large-v3-turbo-q8`

## 方式 A の整形モデル

[google/gemma-4-12b-it](https://huggingface.co/google/gemma-4-12b-it) を [Unsloth が GGUF 化](https://huggingface.co/unsloth/gemma-4-12b-it-GGUF) した `gemma-4-12b-it-Q4_K_M.gguf` を、llama.cpp `b11174` の `llama-gguf-split` で 4 分割したものです。固定リビジョンは `fc034cfff751157913579611efad8462ac1be606`。元の GGUF は 7,121,861,440 bytes、SHA-256 `0a270ec9fe6b34f4a0d33992b6135117b484ebc4766ab76b51d4ae8c457e4c42`。Google の [Gemma 4 モデルカード](https://ai.google.dev/gemma/docs/core/model_card_4) は Apache 2.0 と明記し、Unsloth のモデルカードも `apache-2.0` と表示しています。Unsloth の `license_link` は Google の [Apache License 2.0 全文ページ](https://ai.google.dev/gemma/docs/gemma_4_license) へ転送されます（2026-09-30 確認）。

| ファイル | サイズ (bytes) | SHA-256 |
| --- | ---: | --- |
| `gemma-4-12b-it-Q4_K_M-00001-of-00004.gguf` | 1,812,641,632 | `7a4c2d9d196fd4183a5a12dc934f20048fa729bdf2c5e187106c02b68e78549a` |
| `gemma-4-12b-it-Q4_K_M-00002-of-00004.gguf` | 1,788,424,928 | `47d3ed9fae59885c39c567c3bfb43ade14241831d7d4a1bb963db2a1d4177d99` |
| `gemma-4-12b-it-Q4_K_M-00003-of-00004.gguf` | 1,784,968,256 | `eff6e385bef48cab2ae3fe6117e6363341c83bf3849e01dc868ca4b2c12e90d5` |
| `gemma-4-12b-it-Q4_K_M-00004-of-00004.gguf` | 1,735,827,040 | `fdb769b5dba1d1804a070916041a5fcd75bcd0bb7f5b95af2eb243ad26eef650` |

方式 A の自動取得は試験版 0.9.7 では未実装です。手動導入は、空き容量・保存先・ハッシュ照合を理解した検証者に限って案内します。一般の利用者は方式 B/C を選んでください。

両モデルのライセンス全文は [APACHE-2.0.txt](APACHE-2.0.txt) にあります。

すでに端末にある上級者向けの追加モデルは設定画面に表示される場合があります。追加モデルは配布元の条件がモデルごとに異なるため、試験版では標準認識モデル以外の新規取得を制限しています。手元にあるモデルの利用前には、そのモデルの配布元とライセンスを確認してください。
