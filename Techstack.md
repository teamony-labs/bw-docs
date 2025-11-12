# クマ対策・登山前チェックアプリ 技術スタック

## フロントエンド（モバイルアプリ）
- **フレームワーク**: React Native + Expo
- **UIライブラリ**: HeroUI Mobile
  - ボタン、チェックリスト、カード、タブ、クマキャラ表示など
- **言語**: TypeScript / JavaScript
- **状態管理**: Zustand
  - 行き先情報、持ち物チェック、危険度判定スコアを保持
- **マップ表示（必要に応じて）**: react-native-maps
- **アイコン**: react-native-vector-icons

---

## バックエンド
- **データベース**: Supabase（PostgreSQLベース）
  - 行き先情報（県・山名）
  - クマ出没件数・危険度
  - ユーザーの持ち物チェック状態
  - 危険度判定スコア
- **API通信**: Supabase REST API / GraphQL
- **認証（必要な場合）**: Supabase Auth
- **リアルタイム更新（任意）**: Supabase Realtime

---

## 開発・ビルド
- **開発環境**: Expo CLI + Expo Go
- **ビルド・配布**: ExpoでiOS/Android両方に対応
- **デバッグ**: Expo Goでリアルタイム確認

---

## 特徴・ポイント
- オフライン対応・通知は不要なのでシンプルに開発可能
- HeroUI MobileでUI作成が直感的、デザイン自由度が高い
- Supabaseでデータ管理も簡単、Firebase同等の機能を利用可能
- Zustandでアプリ内の状態管理もシンプル
- 「行き先入力 → 持ち物チェック → 危険度判定」アプリとして十分対応可能

---

## まとめ
- **フロントエンド**: Expo + React Native + HeroUI Mobile + Zustand
- **バックエンド**: Supabase
- この構成で、進級制作用の登山前準備チェックアプリを効率的に開発可能
