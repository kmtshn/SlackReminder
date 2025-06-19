# 🚀 Slack Reminder Generator

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

シンプルで使いやすいSlackリマインダーコマンド生成ツール


## ✨ 特徴

- 🎯 **リアルタイム生成** - 入力と同時にコマンドが自動生成
- 📅 **豊富な間隔設定** - 何分後から毎月まで対応
- 👥 **多様な宛先** - 自分、チャンネル、個別ユーザー対応
- 📱 **レスポンシブデザイン** - モバイル・デスクトップ対応
- 🔄 **依存関係なし** - 外部ライブラリ不要
- 🌐 **日本語対応** - 完全日本語インターフェース

## 🛠️ 対応する間隔設定

| 間隔タイプ | 設定例 | 生成コマンド例 |
|------------|--------|----------------|
| 何分後 | 30分後 | `/remind me "会議準備" in 30 minutes` |
| 何時間後 | 2時間後 | `/remind me "ランチタイム" in 2 hours` |
| 何日後 | 3日後 | `/remind me "プロジェクト確認" in 3 days` |
| 毎日 | 毎日 9:00 | `/remind me "朝礼開始" every day at 9:00 AM` |
| 毎週 | 毎週月曜日 10:00 | `/remind me "週次会議" every Monday at 10:00 AM` |
| 隔週 | 隔週金曜日 17:00 | `/remind me "振り返り" every other Friday at 5:00 PM` |
| 毎月 | 毎月1日 9:00 | `/remind me "月次報告" on the 1st of every month at 9:00 AM` |
| 特定日時 | 2024/12/25 10:00 | `/remind me "クリスマス準備" on December 25, 2024 at 10:00 AM` |

## 🎯 使用方法

### 基本的な使い方

1. **宛先を選択**
   - 自分宛て (`/remind me`)
   - チャンネル宛て (`/remind #channel-name`)
   - 個別ユーザー宛て (`/remind @username`)

2. **間隔を設定**
   - ドロップダウンから間隔タイプを選択
   - 必要に応じて数字、曜日、日付、時間を入力

3. **メッセージを入力**
   - リマインダーの内容を日本語で入力

4. **コマンドをコピー**
   - 自動生成されたSlackコマンドをコピー

5. **Slackで実行**
   - コピーしたコマンドをSlackに貼り付けて実行

### 使用例

#### 即座リマインダー
```bash
# 30分後に自分宛て
/remind me "会議の準備をしてください" in 30 minutes

# 2時間後にチーム宛て
/remind #development "コードレビューの時間です" in 2 hours
```

#### 定期リマインダー
```bash
# 毎日朝9時
/remind me "朝礼開始" every day at 9:00 AM

# 毎週月曜日
/remind #team "週次会議の時間です" every Monday at 10:00 AM

# 毎月1日
/remind me "月次報告書の提出" on the 1st of every month at 9:00 AM
```

#### 個別ユーザー宛て
```bash
# 特定のユーザーに明日リマインド
/remind @tanaka "プロジェクトの進捗確認をお願いします" tomorrow at 2:00 PM
```

## 🚀 セットアップ

### 方法1: GitHub Pagesで公開

1. このリポジトリをクローンまたはフォーク
```bash
git clone https://github.com/your-username/slack-reminder-generator.git
```

2. GitHub Pages を有効化
   - Settings → Pages → Source: Deploy from a branch
   - Branch: main → / (root)

3. アクセス
   - `https://your-username.github.io/slack-reminder-generator/`

### 方法2: ローカル環境で実行

1. ファイルをダウンロード
```bash
wget https://raw.githubusercontent.com/your-username/slack-reminder-generator/main/index.html
```

2. ブラウザで開く
```bash
open index.html
# または
python -m http.server 8000  # Python 3
python -m SimpleHTTPServer 8000  # Python 2
```

### 方法3: 静的ホスティングサービス

以下のサービスで簡単にホスティング可能：
- [Vercel](https://vercel.com/)
- [Netlify](https://www.netlify.com/)
- [GitHub Pages](https://pages.github.com/)
- [Firebase Hosting](https://firebase.google.com/docs/hosting)

## 🏗️ 技術仕様

### 技術スタック
- **HTML5** - セマンティックマークアップ
- **CSS3** - レスポンシブデザイン
- **Vanilla JavaScript** - 外部ライブラリ不要

### ブラウザ対応
- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+

### 特徴的な実装
- リアルタイムコマンド生成
- 動的UI制御（間隔に応じた入力欄の表示/非表示）
- レスポンシブレイアウト
- アクセシビリティ対応

## 🤝 コントリビューション

コントリビューションを歓迎します！

### 貢献方法
1. このリポジトリをフォーク
2. フィーチャーブランチを作成 (`git checkout -b feature/amazing-feature`)
3. 変更をコミット (`git commit -m 'Add some amazing feature'`)
4. ブランチにプッシュ (`git push origin feature/amazing-feature`)
5. プルリクエストを作成

### 開発環境
```bash
# リポジトリをクローン
git clone https://github.com/your-username/slack-reminder-generator.git

# ディレクトリに移動
cd slack-reminder-generator

# 開発サーバーを起動（例：Python）
python -m http.server 8000
```

## 🐛 既知の問題

現在、既知の問題はありません。問題を発見した場合は [Issues](https://github.com/your-username/slack-reminder-generator/issues) でお知らせください。

## 📄 ライセンス

このプロジェクトは [MIT License](LICENSE) の下で公開されています。


## 🙏 謝辞

- Slack API ドキュメント
- MDN Web Docs
- 全てのコントリビューター

---

⭐ このプロジェクトが役に立った場合は、スターをつけていただけると嬉しいです！

## 📞 サポート

質問や問題がある場合：
1. [Issues](https://github.com/your-username/slack-reminder-generator/issues) で問題を報告
2. [Discussions](https://github.com/your-username/slack-reminder-generator/discussions) で質問
](https://ckxlqwqd.gensparkspace.com/)](https://ckxlqwqd.gensparkspace.com/)
