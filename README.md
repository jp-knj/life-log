# life-log

1.5年後の海外転職に向けた日次記録と週次目標管理。

## 使い方

```sh
cd ~/life-log
claude

# 毎晩、歯磨き前
> /log

# 日曜の夜
> /review
> /plan
```

書いたら `git commit && git push`。

## 構造

```
.
├── CLAUDE.md              # ルール・サイクル
├── .claude/commands/
│   ├── log.md             # /log
│   ├── review.md          # /review
│   └── plan.md            # /plan
├── templates/
│   ├── daily.md           # 日次ログテンプレ
│   └── weekly.md          # 週次目標テンプレ
├── goals/
│   └── YYYY-Www.md        # 週次目標
└── logs/
    └── YYYY/MM/
        └── YYYY-MM-DD.md  # 日次ログ
```

## 設計思想

- **記録と解釈を分離**: ログには事実だけ。解釈は週次レビューでだけ行う。
- **3層の目標構造**: Daily Must（床） / Weekly Must / Option B（天井）。Must は希望ではなく確実に届く範囲に置く。
- **習慣化のコストは1つ分**: 5項目を別々に習慣化するのではなく、「毎晩ログを書く」という1つの習慣にすべて乗せる。
- **起床時刻を握る、就寝時刻はデータとして観察**: 就寝は意志でコントロールしづらいので、まず起床側だけ固定する。
