# 1. このリポジトリについて

日本製薬工業協会 データサイエンス部会 2024年度のタスクフォースで作成したプログラム、およびその結果を格納したリポジトリです。詳細は[XXXXXXXXXXXXXXXX](xxxxxxxxxxx)をご参照ください。

このリポジトリで公開しているコードおよびアプリケーションは、成果物の公開時点で使用可能なモデルを選択しています。成果物の作成に使用したモデルとは異なる場合があり、また、将来的にモデルの更新に伴い、公開しているプログラムは実行できなくなる可能性があります。

# 2. リポジトリの構成
<pre>
.
├ 1. CtQF Facilitator
│　　├ 1.1. Develop
│　　└ 1.2. History of communication with AI
│
├ 2. Smart Clinical Data Validator
│　　├ 2.1. Code
│　　├ 2.2. Result_2.5-pro-exp-03-25
│　　└ 2.3. updated_files_csv
│
├ LICENSE
└ README.md
</pre>

# 3. 格納されているファイルについて
## 1. CtQF Facilitator
- Critical to Quality Factorの特定を支援する対話型AIの設定ファイルと、その実行ログを格納しています。
- DifyとGeminiを連携しているため、再現にはDifyのアカウントとGeminiのAPI Keyが必要です。

### 1.1. Develop
- Difyの設定ファイル（yml）ファイルを格納しています。
- 対話型AIを再現するための手順：
  - [Dify](https://dify.ai/)でアカウントを作成します。
  - Difyの設定からGeminiを追加し、API Keyを設定します。
  - このフォルダにあるDSL.ymlをDSLとしてインポートします。
  - 「知識習得」のブロックで以下の3つをナレッジとして指定します。
     - https://ctti-clinicaltrials.org/about/ctti-projects/quality-by-design/qbd-quality-by-design-toolkit/exploring-the-critical-to-quality-ctq-factors/
     - https://ctti-clinicaltrials.org/wp-content/uploads/2021/07/CTTI_QbD_Workshop_Principles_Document-1.pdf
     - https://pmc.ncbi.nlm.nih.gov/articles/PMC10276776/pdf/43441_2023_Article_504.pdf

### 1.2. History of communication with AI
- タスクフォースで実施した会話のログを、Wordファイルで格納しています。

### Note: タスクフォースで作成したサンプルアプリ
- こちらのリンクで公開しています：https://udify.app/chat/8wpsRKU9mspQvuGL
- テスト目的であれば、自己の責任においてご自由にお試しいただけます。
- 出力内容は大規模言語モデルによるものであり、誤った内容が出力される可能性がある点にご留意ください。
- すべての実行ログはDifyのサーバーに記録され、アップロードしたファイルもDifyサーバーで管理されます。
- **誤ったファイルをアップロードした場合、ファイルは削除することができません。**

　

## 2. Smart Clinical Data Validator
- 臨床試験データをレビューするAIのプログラムと、その実行ログを格納しています。
- プログラムの実行にはGoogleアカウントとGeminiのAPI Keyが必要です。

### 2.1. Code
 - このフォルダにあるCode.ipynbが実行プログラムです。
 - <img src ="https://github.com/Takumi173/JPMA2022TF1-1/assets/109738801/522a6fd7-b171-4ad3-8f56-e73a718a6542">のアイコンをクリックすることでColaboratoryで開けます。
 - 使用しているプロンプトはプログラム内でご確認いただけますが、同様の内容をPromptフォルダにも格納しています。

### 2.2. Result_2.5-pro-exp-03-25
 - 対象とした症例のレビュー結果は、レビュー結果.mdにまとめています。
 - 個別の症例の状況について問い合わせた結果は、00-000-0000の見解.mdというファイル名で格納しています。

### 2.3. updated_files_csv
 - 実行プログラムの中で更新した、更新後の全データを格納しています。

　

# 4. 免責事項
プログラムの作者および製薬協は、本リポジトリで公開されているプログラムの実行によって生じたいかなる損害に対して、一切の責任を負いません。

# 5. ライセンス
このリポジトリにあるコードは、MITライセンスの下に配布されます。
