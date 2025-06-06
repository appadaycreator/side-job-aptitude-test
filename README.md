# 副業適性診断テスト - Web公開ガイド

## 📋 概要
10の質問でユーザーの副業適性を診断し、TOP3の副業を提案するWebサービスです。

## 🚀 Web公開手順（GitHub Pages）

### 1. GitHubリポジトリ作成
```bash
# GitHubにログイン後、新しいリポジトリを作成
リポジトリ名: side-job-aptitude-test
説明: 副業適性診断テスト - あなたにピッタリの副業が見つかる
公開設定: Public
```

### 2. ファイルのアップロード
以下のファイルをリポジトリにアップロード：
- `index.html` - メインのHTMLファイル
- `sitemap.xml` - サイトマップ
- `robots.txt` - クローラー制御ファイル

### 3. GitHub Pages有効化
1. リポジトリの Settings タブをクリック
2. 左サイドバーの「Pages」をクリック
3. Source で「Deploy from a branch」を選択
4. Branch で「main」を選択
5. Folder で「/ (root)」を選択
6. Save をクリック

### 4. 公開URL確認
- 約5-10分後に以下のURLでアクセス可能
- `https://appadaycreator.github.io/side-job-aptitude-test/`

## 📊 Google Analytics設定

### 1. Google Analytics 4 設定
1. [Google Analytics](https://analytics.google.com/)にアクセス
2. 新しいプロパティを作成
3. プロパティ名: 「副業適性診断テスト」
4. 測定ID (G-XXXXXXXXXX) を取得

### 2. Google Tag Manager設定
- 既にHTMLファイルに実装済み（GTM-TXQGZRF9）
- Google Tag Managerで以下を設定：
  - Google Analytics 4 の設定
  - 診断完了イベントの追跡
  - ボタンクリック追跡
  - スクロール追跡

## 🔍 Google Search Console設定

### 1. プロパティ追加
1. [Google Search Console](https://search.google.com/search-console/)にアクセス
2. 「プロパティを追加」をクリック
3. 「URLプレフィックス」を選択
4. URL: `https://appadaycreator.github.io/side-job-aptitude-test/`

### 2. 所有権確認
- HTMLファイル方式での確認推奨
- ダウンロードしたファイルをリポジトリルートに配置

### 3. サイトマップ送信
1. 「サイトマップ」メニューを選択
2. サイトマップURL: `sitemap.xml` を入力
3. 送信をクリック

## 💰 アフィリエイト設定

### A8.net サイト登録
- **サイト名**: 副業適性診断テスト
- **サイト紹介文**: あなたにピッタリの副業を見つける無料診断サービス。10の質問でスキルと時間に合った副業TOP3を提案し、月5万円の副収入実現をサポートします。

### 推奨アフィリエイト案件
1. **クラウドワークス** - クラウドソーシング
2. **ココナラ** - スキルマーケット  
3. **Udemy** - オンライン学習
4. **ランサーズ** - フリーランス支援
5. **楽天市場** - 副業関連書籍・ツール

## 📱 機能説明

### 実装済み機能
- ✅ 10問の診断テスト
- ✅ TOP3副業提案
- ✅ 適合度レーダーチャート
- ✅ SNSシェア機能（X, LINE）
- ✅ 友達との比較機能
- ✅ 診断履歴保存（LocalStorage）
- ✅ レスポンシブデザイン
- ✅ Google Tag Manager統合

### 診断ロジック
- スキルレベル、時間、収入目標等10項目を重み付けスコアリング
- 10種類の副業データベースとマッチング
- 適合度を0-100%で算出

## 🔧 カスタマイズ方法

### 副業データベース追加
`jobDatabase` 配列に新しい副業情報を追加可能：
```javascript
{
    title: "新しい副業",
    skills: ["必要スキル"],
    timeRequired: "minimal/moderate/substantial",
    incomeRange: "収入範囲",
    difficulty: "beginner/intermediate/advanced",
    description: "説明",
    requirements: "必要条件",
    startingSteps: "始め方"
}
```

### デザインカスタマイズ
CSS変数で簡単にテーマ変更：
```css
:root {
    --primary-color: #38b2ac;
    --secondary-color: #667eea;
    --text-color: #2d3748;
}
```

## 📈 SEO最適化

### 実装済みSEO対策
- メタタグ設定（title, description, OGP）
- 構造化データ対応
- パフォーマンス最適化
- モバイルフレンドリー対応
- セマンティックHTML

### 推奨SEOキーワード
- 副業適性診断
- 副業診断テスト  
- 在宅ワーク適性
- スキル診断
- 副業おすすめ

## 🚨 注意事項

### ブラウザストレージ制限
- LocalStorageを使用（データはブラウザローカルに保存）
- ユーザーがブラウザデータを削除すると履歴も消失

### アフィリエイトリンク更新
- A8.netやその他のアフィリエイトリンクは実際のものに更新してください
- 現在はサンプルURLが設定されています

### プライバシーポリシー
- 今後、診断データの取り扱いについてプライバシーポリシーページの追加を推奨

## 📞 サポート
何か問題があれば、GitHubのIssueまたは @appadaycreator までご連絡ください。