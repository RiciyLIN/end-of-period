# 📅 日々のリマインダー (Hibi Reminder)

> シンプルで使いやすい、日本語対応のWebリマインダーアプリ。  
> 予定管理と天気情報が一体となった、毎日を快適にサポートします。

---

## 🎨 デザインコンセプト

- **ミニマル＆クリーン**：無駄を省いたすっきりとしたUIで、誰でも直感的に操作可能  
- **日本語フォーカス**：和風の親しみやすさを意識した日本語対応・曜日表示  
- **レスポンシブ対応**：スマホ・タブレット・PCで快適に閲覧・操作可能  
- **色彩設計**：青系のアクセントカラーで清潔感と信頼感を演出

---

## 🚀 主な機能

- 🔒 **Firebase認証**で安心のログイン・新規登録機能  
- 📅 **7日間の予定表示と編集**  
- 🕑 時間付きリマインダーの追加・削除  
- 🌤️ **現在地・指定日の天気予報表示**（OpenWeatherMap API利用）  
- 📱 **モバイルファースト設計**  
- 🔄 ログアウトボタン搭載

---

## 🛠️ 使用技術スタック

| 技術                   | 用途                             |
|------------------------|----------------------------------|
| HTML / CSS / JS        | フロントエンドUIと操作ロジック  |
| Firebase Authentication | ユーザー管理（ログイン・登録）   |
| Firebase Firestore     | リマインダーのデータ保存         |
| OpenWeatherMap API     | 天気情報取得                     |

---

## 💻 ローカルでの動作確認方法

1. このリポジトリをクローンまたはダウンロード  
2. Firebaseプロジェクトの設定情報を `index.html`, `login.html`, `register.html` の `firebaseConfig` に反映  
3. Webサーバーでファイルを配信（Live Serverや簡易HTTPサーバー推奨）  
4. ブラウザで `login.html` からアクセスし、アカウント登録→ログイン→リマインダー管理

---

## 🔐 APIキー・機密情報の設定について

このアプリでは、Firebase および OpenWeatherMap の Web API を使用しています。**セキュリティ保護のため、GitHub 上には実際の API キー等を公開していません。**

### Firebase の設定方法

Firebase コンソールから自身のプロジェクトを作成し、以下の形式で各 HTML ファイルの `firebaseConfig` に記入してください：

```javascript
const firebaseConfig = {
  apiKey: "あなたの Firebase APIキー",
  authDomain: "あなたの Firebase 認証ドメイン",
  projectId: "あなたの Firebase プロジェクトID",
};
````

### OpenWeatherMap の設定方法

[OpenWeatherMap](https://openweathermap.org/api) に無料登録して APIキーを取得し、以下のように記入してください：

```javascript
const apiKey = "あなたの OpenWeatherMap APIキー";
```

> 🔒 **注意：これらのキーを GitHub にアップロードしないでください。**

---

## 📝 画面構成

| ページ             | 内容                     |
| --------------- | ---------------------- |
| `login.html`    | メールアドレス・パスワードでログイン     |
| `register.html` | 新規アカウント登録              |
| `index.html`    | メイン画面。リマインダー一覧・追加・天気表示 |

---

## ✨ 今後の展望

* プッシュ通知対応
* カレンダー連携（Googleカレンダー等）
* リマインダーの繰り返し設定
* UIのテーマ切替（ライト/ダークモード）

---

© 2025 日々のリマインダー
Designed & Developed by XY LIN

---


