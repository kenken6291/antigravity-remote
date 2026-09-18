# Antigravity 外出先指示システム (所有者限定認証付き)

## 🔒 アクセス制限仕様
- **対象ドメイン**: `https://kenken6291.github.io/antigravity-remote/`
- **許可アカウント**: **`aksaginuma@gmail.com`** 限定

---

## 🛡 認証・アクセス制御の仕組み
1. **Google Identity (Sign in with Google) ログイン**:
   - `https://kenken6291.github.io/antigravity-remote/` にアクセスすると、まず認証画面（ログインカード）が表示されます。
2. **所有者メールアドレス判定**:
   - Google アカウントでログインした際、メールアドレスが `aksaginuma@gmail.com` であるか判定します。
   - 一致しない場合は「⛔ アクセス拒否」となり、リモコン操作画面が開かないよう自動ブロックされます。
3. **バックエンド API 認可**:
   - GAS (`gas/Code.gs`) 側でも `aksaginuma@gmail.com` の検証を行い、不正なリクエストを防止します。

---

## 📂 更新ファイルの配置
- **GitHub Pages 用画面**: [github_pages/index.html](file:///g:/%E3%83%9E%E3%82%A4%E3%83%89%E3%83%A9%E3%82%A4%E3%83%96/%E5%81%A5%E4%BA%8C%E4%BF%9D%E7%AE%A1%E5%BA%AB/15_Antigravity/github_pages/index.html)
- **GAS バックエンド**: [gas/Code.gs](file:///g:/%E3%83%9E%E3%82%A4%E3%83%89%E3%83%A9%E3%82%A4%E3%83%96/%E5%81%A5%E4%BA%8C%E4%BF%9D%E7%AE%A1%E5%BA%AB/15_Antigravity/gas/Code.gs)
