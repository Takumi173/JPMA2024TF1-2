# このリポジトリについて

日本製薬工業協会 データサイエンス部会 2024年度のタスクフォースで作成したプログラム、およびその結果を格納したリポジトリです。詳細は[XXXXXXXXXXXXXXXX](xxxxxxxxxxx)をご参照ください。

# 実行環境

### 1. CtQF Facilitator
- Critical to Quality Factorの特定を支援する対話型AIです
- DifyとGeminiを連携させています。
- 再現するためにはDifyのアカウントとGeminiのAPI Keyが必要です。
      
### 2. Smart Clinical Data Validator
- 臨床試験データをレビューするAIです。
- [Colaboratory](https://colab.research.google.com/?hl=ja)で実行します。
- 実行にはGoogleアカウントとGeminiのAPI Keyが必要です。

# 免責事項
プログラムの作者および製薬協は、本リポジトリで公開されているプログラムの実行によって生じたいかなる損害に対して、一切の責任を負いません。

# ライセンス
このリポジトリにあるコードは、MITライセンスの下に配布されます。



# Developフォルダ
以下の手順で対話型AIを再現できます
- [Dify](https://dify.ai/)でアカウントを作成します。
- Difyの設定からGeminiを追加し、API Keyを設定します。
- このフォルダにあるDSL.ymlをDSLとしてインポートします。
- 「知識習得」のブロックで以下の3つをナレッジとして指定します。
   - https://ctti-clinicaltrials.org/about/ctti-projects/quality-by-design/qbd-quality-by-design-toolkit/exploring-the-critical-to-quality-ctq-factors/
   - https://ctti-clinicaltrials.org/wp-content/uploads/2021/07/CTTI_QbD_Workshop_Principles_Document-1.pdf
   - https://pmc.ncbi.nlm.nih.gov/articles/PMC10276776/pdf/43441_2023_Article_504.pdf

# History of communication with AIフォルダ
- タスクフォースで実施した会話のログを、Wordファイルに変換してに格納しています。

# サンプルアプリ
- リンク：https://udify.app/chat/8wpsRKU9mspQvuGL
- テスト目的であれば、サンプルアプリは自己責任でご自由にお試しいただいて構いません。
- すべての実行ログはDifyサーバーに記録され、アップロードファイルもDifyサーバーで管理されます。
- **誤ったファイルをアップロードしても、ファイルは削除することができません。**
- 出力内容は大規模言語モデルによるものであり、誤った内容が出力される可能性があります。


# Codeフォルダ
このフォルダにあるCode.ipynbがプログラムです。

<img src ="https://github.com/Takumi173/JPMA2022TF1-1/assets/109738801/522a6fd7-b171-4ad3-8f56-e73a718a6542">のアイコンをクリックすることでColaboratoryで開けます。

Promptフォルダでは、Code.ipynb内で使用しているシステムプロンプトとユーザープロンプトを切り出し、閲覧用に格納しています。

# Result_2.5-pro-exp-03-25フォルダ
対象とした症例のレビュー結果を、レビュー結果.mdにまとめています。

個別の症例の状況について問い合わせた内容は、それぞれの症例の見解として個別に格納しています。
