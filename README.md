# 🎈 Streamlit + LLM サンプルアプリ

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/kun432/streamlit-llm-examples?quickstart=1)

Streamlit で LLM アプリを構築するためのスターターサンプルです。

## アプリ概要

このアプリには、LLM のミニマムな実装例を随時追加しています。

現在利用できるサンプル:

- チャットボット
- ファイル Q&A
- インターネット検索付きチャット
- LangChain クイックスタート
- LangChain PromptTemplate
- フィードバック入力付きチャット

## デモアプリ

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://llm-examples.streamlit.app/)

### OpenAI API キーを取得する

以下の手順で OpenAI API キーを取得できます。

1. https://platform.openai.com/account/api-keys にアクセスします。
2. `+ Create new secret key` をクリックします。
3. 識別名（任意）を入力し、`Create secret key` をクリックします。

### Streamlit Community Cloud に OpenAI API キーを設定する

Streamlit アプリで環境変数として OpenAI API キーを設定するには、以下を行います。

1. 画面右下の `< Manage app` をクリックし、縦三点リーダー「...」から `Settings` を開きます。
2. 表示された **App settings** で `Secrets` タブを開き、次のように API キーを貼り付けます。

```sh
OPENAI_API_KEY='xxxxxxxxxx'
```

## ローカルで実行する

`uv`が必要です。

```sh
uv sync
uv run pre-commit install
uv run streamlit run Chatbot.py
```
