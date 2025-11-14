# 🤖 AI専門家相談アプリ

## 📋 概要
このアプリは、様々な分野の専門家AIとチャットできるWebアプリです。LangChainとOpenAI GPT-4o-miniを使用し、選択した専門分野に特化した回答を提供します。

## ✨ 機能
- 🎯 **専門家選択**: プログラミング、料理、旅行、健康・フィットネス、ビジネスの専門家から選択
- 💬 **インタラクティブチャット**: 選択した専門家に特化した質問・相談が可能
- 🎨 **直感的UI**: Streamlitによる使いやすいWebインターフェース
- ⚡ **高速レスポンス**: OpenAI GPT-4o-miniによる迅速な回答生成

## 🛠️ 技術スタック
- **Frontend**: Streamlit
- **LLM**: OpenAI GPT-4o-mini
- **Framework**: LangChain
- **Python Version**: 3.11
- **Deployment**: Streamlit Community Cloud

## 🚀 ローカル実行方法

### 前提条件
- Python 3.11+
- OpenAI APIキー

### セットアップ手順

1. **リポジトリのクローン**
```bash
git clone https://github.com/your-username/streamlit-llm-app.git
cd streamlit-llm-app
```

2. **仮想環境の作成と有効化**
```bash
python -m venv env
# Windows
env\Scripts\activate
# macOS/Linux
source env/bin/activate
```

3. **依存関係のインストール**
```bash
pip install -r requirements.txt
```

4. **環境変数の設定**
```bash
# .env.exampleを.envにコピー
cp .env.example .env
# .envファイルを編集してOPENAI_API_KEYを設定
```

5. **アプリの実行**
```bash
streamlit run app.py
```

## 🌐 デプロイメント (Streamlit Community Cloud)

1. GitHubリポジトリをStreamlit Community Cloudに接続
2. OpenAI APIキーをSecrets管理で設定:
   - Key: `OPENAI_API_KEY`
   - Value: あなたのOpenAI APIキー
3. デプロイ実行

## 📁 ファイル構造
```
streamlit-llm-app/
├── app.py              # メインアプリケーション
├── requirements.txt    # 依存関係
├── runtime.txt        # Python バージョン指定
├── .env.example       # 環境変数テンプレート
└── README.md          # このファイル
```

## 🎯 使用方法
1. 専門家を選択（プログラミング、料理、旅行、健康・フィットネス、ビジネス）
2. 質問や相談内容をテキストエリアに入力
3. 「回答を取得」ボタンをクリック
4. 選択した専門家からの回答を確認

## ⚠️ 注意事項
- OpenAI APIキーが必要です
- API使用料が発生する場合があります
- 回答の生成には数秒かかる場合があります

## 📄 ライセンス
このプロジェクトはMITライセンスのもとで公開されています。