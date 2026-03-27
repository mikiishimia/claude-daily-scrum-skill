# config.example.md
# このファイルをコピーして config.md にリネームし、自分の情報を記入してください。
# config.md は .gitignore に追加して個人情報を保護してください。

---

## 基本情報

```
NAME: あなたの名前（例：田中太郎）
TIMEZONE: Asia/Tokyo
```

---

## 就業時間

```
WORK_HOURS:
  start: "12:00"    # 就業開始時刻
  end: "18:00"      # 就業終了時刻
  deep_work: "12:00-15:00"   # 集中作業（執筆・創造系）
  light_work: "15:00-17:00"  # 連絡・営業系
  buffer: "17:00-18:00"      # バッファ
```

---

## Notion

```
BACKLOG_URL: https://www.notion.so/YOUR_WORKSPACE/YOUR_BACKLOG_PAGE_ID
DAILY_ACTION_DB: YOUR_DAILY_ACTION_DATABASE_ID
ATTACK_LIST_DB: YOUR_ATTACK_LIST_DATABASE_ID  # 営業パイプラインを使う場合
```

---

## Gmail 優先チェックドメイン

営業パイプラインで重点確認したい企業・クライアントのドメインを記入

```
GMAIL_PRIORITY_DOMAINS:
  - example.com
  - client1.co.jp
  - client2.com
```

---

## 営業パイプライン（使わない場合は削除可）

```
PIPELINE_STAGES:
  - 未判定
  - ◎判定
  - アプローチ済
  - 返信あり
  - 面談
  - 提案
  - 契約

TARGET_CRITERIA: |
  自分のターゲット顧客の定義を記入する。
  例：シリーズA/B、PMF達成済み、社内デザイナーなし、技術力高め
```

---

## 仕事リズム（任意）

Daily Scrumのタイムブロック提案を最適化するために記入

```
WORK_STYLE: |
  - 創造系タスクは就業直後が得意
  - 体調が悪い日はタスクを2個に絞る
  - やりたくないタスクは30分以内に区切る
  - （自分のリズムを自由に記述）

AVOID_SUGGESTIONS: |
  - 対面イベント  # 参加できない条件があれば記述
```

---

## .gitignore への追加（必須）

このファイルを参考に、実際の config.md は必ずGitから除外してください：

```
# .gitignore
config.md
```
