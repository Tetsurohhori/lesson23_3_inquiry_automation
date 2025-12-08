# 問い合わせ対応自動化AIエージェント

このプロジェクトは、顧客からの問い合わせに自動で対応し、適切な担当者にSlack通知を送るAIエージェントシステムです。

## 機能

- RAG（Retrieval-Augmented Generation）による社内文書参照
- AIエージェントによる自動回答生成
- 問い合わせ内容に応じた担当者の自動割り振り
- Slackへの自動通知とメンション

## セットアップ

### 必要な環境変数

以下の環境変数を設定してください：

- `OPENAI_API_KEY`: OpenAI APIキー
- `SERPAPI_API_KEY`: SerpAPI APIキー（Web検索用）
- `SLACK_BOT_TOKEN`: Slack Botトークン
- `SLACK_APP_TOKEN`: Slack Appトークン

### ローカル実行

```bash
cd "ダウンロード用/Slack連携あり/customer-contact"
streamlit run main.py
```

## 使用技術

- Python 3.11
- Streamlit
- LangChain
- OpenAI GPT-4
- ChromaDB
- Slack SDK
