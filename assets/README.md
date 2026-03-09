# アセット命名ルール / Asset Naming Convention

画像・SVGは **「使用箇所が分かる読みやすい名前」** で統一しています。

## フォルダ構成

- **`png/`** … 画像（PNG）
- **`svg/`** … ベクターアイコン・ロゴ（SVG）

## ルール: `{section}_{role}_{description}.{ext}`

- **section** … 使われている画面・ブロック（fv / main / feature / badge / story）
- **role** … 役割（hero, background, screenshot, profilecard など）
- **description** … 内容の補足（01〜04, income, career など）
- 英小文字・数字・アンダースコアのみ使用

## セクション略称

| 略称 | セクション |
|------|------------|
| `fv` | First View（ヒーロー） |
| `main` | Main（基準を下げない出会い） |
| `feature` | Feature（特徴・4枚のカード） |
| `badge` | Screening & Badge System（審査・バッジ） |
| `story` | Story（信頼できる出会いのため） |

## PNG 一覧（`png/` 内・使用箇所）

| ファイル名 | 使用箇所 |
|------------|----------|
| `fv_hero_background.png` | FV ヒーロー背景 |
| `main_couple_background.png` | Main ブロック背景（カップル写真） |
| `feature_01_screening_screenshot.png` | Feature カード1：書類確認を伴う審査制度 |
| `feature_02_badge_profilecard.png` | Feature カード2：「バッジ」で証明された価値 |
| `feature_03_lounge_profilecard.png` | Feature カード3：ラウンジ機能 |
| `feature_04_dailycard_profilecard.png` | Feature カード4：デイリーカード |
| `badge_income.png` | バッジカルーセル：収入認証バッジ |
| `badge_career.png` | バッジカルーセル：キャリア認証バッジ |
| `badge_asset.png` | バッジカルーセル：資産認証バッジ |
| `badge_male_criteria_illust.png` | 男性の登録基準カード内イラスト |
| `badge_male_criteria_illust_02.png` | 予備・別パターン用 |
| `story_background.png` | Story ブロック背景 |

## SVG（`svg/` 内）

アイコン・ロゴ用の SVG は `svg/` フォルダ内にハッシュ名で保存されています。  
使用する際は必要に応じて `fv_`, `badge_` などのプレフィックスでリネームしてください。
