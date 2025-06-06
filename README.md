# 桜町中学校1976年卒業同窓会 ホームページ

## 概要
桜町中学校1976年卒業生の同窓会ホームページです。同窓生同士の交流と情報共有を目的としています。

## サイト構成

### 一般公開ページ
- **index.html** - トップページ
- **about.html** - 同窓会について
- **contact.html** - お問い合わせ

### 会員専用ページ
- **members.html** - 会員専用ページ（パスワード保護）
  - お知らせ・イベント情報
  - 写真ギャラリー
  - 交流掲示板
  - 名簿情報

### スタイル・設定ファイル
- **styles.css** - 全体のスタイルシート

## 特徴

### デザイン
- レスポンシブデザイン（スマホ対応）
- 清潔感のあるブルー系カラー
- 読みやすいフォント設定

### 機能
- パスワード保護による会員制
- 出欠確認フォーム
- 交流掲示板
- 写真ギャラリー
- 名簿情報管理

## 🚀 デプロイ方法

### EmailJS設定（必須）

デプロイ前にEmailJS設定ファイルを作成してください：

1. `assets/js/emailjs-config.template.js` をコピーして `assets/js/emailjs-config.js` を作成
2. 実際のEmailJS設定値を入力：
   ```javascript
   window.EMAILJS_CONFIG = {
       serviceId: 'your_actual_service_id',
       publicKey: 'your_actual_public_key',
       templateIds: {
           admin_notification: 'your_actual_template_id'
       }
   };
   ```

### セキュリティ設定

- `assets/js/emailjs-config.js` は `.gitignore` で除外済み
- 本番環境では環境変数での設定を推奨
- APIキーは絶対にGitHubにコミットしないでください

## GitHub Pagesでの公開手順

### 1. GitHubアカウント作成
1. https://github.com にアクセス
2. 「Sign up」でアカウント作成

### 2. リポジトリ作成
1. 「New repository」をクリック
2. Repository name: `sakuramachi-1976`
3. 「Public」を選択
4. 「Create repository」をクリック

### 3. ファイルアップロード
1. 「uploading an existing file」をクリック
2. 以下のファイルをドラッグ&ドロップ:
   - index.html
   - about.html
   - contact.html
   - members.html
   - styles.css
   - README.md
3. 「Commit changes」をクリック

### 4. GitHub Pages設定
1. リポジトリの「Settings」タブをクリック
2. 左メニューの「Pages」をクリック
3. Source: 「Deploy from a branch」
4. Branch: 「main」を選択
5. 「Save」をクリック

### 5. サイトURL確認
数分後、以下のURLでアクセス可能になります：
```
https://[あなたのユーザー名].github.io/sakuramachi-1976/
```

## パスワード設定

### 現在のパスワード
- **パスワード**: `sakura1976`

### パスワード変更方法
1. `members.html` の23行目を編集:
   ```javascript
   const correctPassword = "新しいパスワード";
   ```
2. ファイルをGitHubに再アップロード

## 運用のポイント

### 内容更新
1. HTMLファイルを編集
2. GitHubリポジトリに再アップロード
3. 数分で反映

### 写真追加
1. 写真ファイルをGitHubにアップロード
2. `members.html` の写真ギャラリー部分を編集
3. 画像パスを更新

### お知らせ更新
1. `members.html` のお知らせセクションを編集
2. 日付と内容を更新

## セキュリティ注意事項

1. **パスワード管理**: 定期的にパスワードを変更
2. **個人情報**: 名簿情報は最小限に留める
3. **写真**: 掲載許可を事前に取得
4. **バックアップ**: 定期的にファイルをバックアップ

## サポート

### 技術的な質問
- HTMLの編集方法
- GitHubの使い方
- サイトの機能追加

### 運用に関する質問
- 内容の更新方法
- 新機能の追加
- デザインの変更

お困りの際は、お気軽にお問い合わせください。

## 更新履歴

- 2025/01/XX - 初回リリース
- 基本ページ作成
- パスワード保護機能実装
- レスポンシブデザイン対応

---

**桜町中学校1976年卒業同窓会事務局**