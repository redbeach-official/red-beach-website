# RED BEACH合同会社 ウェブサイトデプロイ完了レポート

**作成日**: 2025年11月27日  
**プロジェクト**: RED BEACH合同会社 公式ウェブサイト  
**ドメイン**: https://red-beach.com

---

## デプロイ概要

WIXから自社ホスティング（GitHub Pages）への移行が完了しました。

---

## 完了した作業

### 1. GitHubリポジトリの作成
- **リポジトリ名**: `redbeach-official/red-beach-website`
- **公開設定**: Public
- **リモートURL**: https://github.com/redbeach-official/red-beach-website

### 2. ビルドとデプロイ
- **ビルドツール**: Vite
- **フレームワーク**: React 19
- **スタイリング**: Tailwind CSS 4
- **デプロイ先**: GitHub Pages

### 3. カスタムドメイン設定
- **ドメイン**: red-beach.com
- **DNS設定**: お名前.comで設定済み
  - A レコード: GitHub PagesのIPアドレス
  - CNAME レコード: www → red-beach.com
- **SSL証明書**: 自動発行（有効期限: 2026年2月16日）
- **HTTPS強制**: 有効

### 4. メール設定（既存）
- **メールアドレス**: t.hama@red-beach.com
- **メールサーバー**: Sakura Internet
- **転送先**: redbeach.hama@gmail.com

### 5. お問い合わせフォーム
- **サービス**: Formspree
- **フォームID**: meqavdlj
- **送信先**: redbeach.hama@gmail.com

---

## ウェブサイト構成

### ページ一覧

1. **HOMEページ** (`/`)
   - 会社紹介
   - 事業内容の説明
   - お問い合わせボタン

2. **COMPANYページ** (`/company`)
   - 会社概要
   - 社名、設立日、代表者名
   - 所在地、事業内容
   - 適格請求書発行事業者番号

3. **CONTACTページ** (`/contact`)
   - お問い合わせフォーム
   - Formspree連携

---

## 技術スタック

| 項目 | 技術 |
|------|------|
| **ホスティング** | GitHub Pages |
| **ドメイン** | red-beach.com（お名前.com） |
| **フロントエンド** | React 19 + Vite |
| **スタイリング** | Tailwind CSS 4 |
| **フォーム** | Formspree |
| **メールサーバー** | Sakura Internet |
| **SSL証明書** | GitHub Pages自動発行 |

---

## コスト比較

### WIX（移行前）
- **プレミアムプラン**: ¥30,360/年
- **メールボックス**: ¥10,560/年
- **ドメイン**: ¥4,316/年
- **合計**: **¥45,236/年**

### GitHub Pages（移行後）
- **ホスティング**: 無料
- **ドメイン**: ¥4,316/年（お名前.com）
- **メールサーバー**: ¥1,571/年（Sakura Internet）
- **Formspree**: 無料プラン
- **合計**: **¥5,887/年**

### **年間削減額: ¥39,349**

---

## アクセスURL

- **メインドメイン**: https://red-beach.com
- **wwwサブドメイン**: https://www.red-beach.com
- **GitHubリポジトリ**: https://github.com/redbeach-official/red-beach-website

---

## 今後のメンテナンス

### ウェブサイト更新方法

1. ローカルでファイルを編集
2. `pnpm run build` でビルド
3. `dist/public/` の内容をGitHubリポジトリにプッシュ

### 必要な認証情報

- **GitHub Personal Access Token**: 90日ごとに更新が必要
- **Formspree アカウント**: redbeach.hama@gmail.com

---

## 確認事項

✅ ウェブサイトが https://red-beach.com で正常に表示  
✅ SSL証明書が有効  
✅ すべてのページ（HOME、COMPANY、CONTACT）が動作  
✅ お問い合わせフォームが機能  
✅ メール受信が正常に動作  
✅ レスポンシブデザイン対応  

---

## 注意事項

1. **Personal Access Tokenの有効期限**
   - 作成日: 2025年11月27日
   - 有効期限: 2026年2月25日（90日後）
   - 期限前に新しいトークンを作成してください

2. **DNS設定**
   - お名前.comでDNS設定を変更しないでください
   - 変更が必要な場合は、GitHub Pagesの設定も確認してください

3. **メール送信**
   - SPFレコードのDNS伝播が完了するまで、Gmailからのメール送信が失敗する可能性があります
   - 24-48時間後に再度テストしてください

---

## サポート

ウェブサイトの更新やメンテナンスに関するご質問は、Manusまでお問い合わせください。

---

**デプロイ完了日時**: 2025年11月27日 22:06  
**担当**: Manus AI Assistant
