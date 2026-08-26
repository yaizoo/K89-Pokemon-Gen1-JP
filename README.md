# K89 Pokémon Gen1 JP

Gen1Recomp版『Pokémon Red / Blue』を、オリジナル日本版の雰囲気に近づけるための非公式日本語化MODです。

**K89 Pokémon Gen1 JP** は、Gen1Recompで動作する英語版『Pokémon Red / Blue』を、日本版Generation Iのテキスト・UI・タイトル画面・名称・グラフィック表現に近づけることを目的としています。

単純な機械翻訳ではなく、原作日本版の文章・名称・表示形式を基準に実装しています。

## 対応ゲーム

- Pokémon Red
- Pokémon Blue

Pokémon Yellowには現在対応していません。

## 現在のバージョン

**v0.6.0**

対応ランタイム：

**Gen1Recomp 0.1.89+**

## 主な特徴

- ゲーム内テキストの日本語化
- 日本語版Generation Iに近いかなフォント表示
- 濁点・半濁点表示
- ポケモン名の日本語化
- わざ名の日本語化
- アイテム名の日本語化
- トレーナー名の日本語化
- マップ名の日本語化
- メニュー・名前入力画面の日本語化
- Pokédex・Trainer Card・Fly・Safari ZoneなどのUI日本語化
- バトルHUD・状態表示の日本語化
- 日本版Red / Blueのタイトル画面表現
- Red / Blue固有テキストへの対応
- Pokémon Red用の日本版ポケモンスプライト
- 他の表示MODとの互換性を考慮したスプライト処理

## Pokémon Blue

BlueではK89の日本語テキスト、UI、名称、フォント、タイトル画面などを適用します。

**Blueのゲーム中ポケモンスプライトは変更しません。**

K89のPokémon sprite hookはBlueでは置換処理を行わず、Gen1Recomp標準のBlueスプライトをそのまま使用します。

## Pokémon Red

Redでは共通の日本語化に加えて、日本版Red固有の内容を適用します。

主なRed専用対応：

- 日本版Red v1.1のPokédex文章151件
- Red固有のゲーム内交換会話差分
- 日本版Redタイトル画面
- 日本版Redトレーナー／プレイヤーグラフィック
- 日本版Redのポケモンスプライト

Redを起動している場合のみ、MOD設定に以下の項目が表示されます。

`JP RED SPRITES`

**ON**

日本版Pokémon Redのポケモンスプライトを使用します。

**OFF**

Gen1Recomp標準のポケモンスプライトを使用します。

この設定はPokémon Blueでは表示されません。

## v0.6.0

v0.6.0では、従来の **K89 Pokémon Blue JP** をRed / Blue共通のGeneration I日本語化MODへ拡張しました。

主な変更：

- Pokémon Redに正式対応
- Red / Blue共通の日本語化ランタイムを統合
- 日本版Red v1.1 Pokédex文章151件を追加
- Red固有のゲーム内交換テキスト差分を追加
- 日本版Redタイトル画面を追加
- 日本版Redトレーナー／プレイヤーグラフィックを追加
- 日本版Redポケモンスプライト151体分を追加
- Red専用 `JP RED SPRITES` オプションを追加
- Blueではポケモンスプライト置換処理を完全に無効化
- Gen1Recompの `pokemon.sprite` hookを利用したスプライト処理に対応
- Dramatic Shapeなど、表示方向を変更するMODとの共存を考慮
- 従来のK89 Pokémon Blue JP v0.5.5の日本語化・UI監査内容を統合

## 日本語化の方針

このMODは英語版テキストをそのまま日本語へ翻訳したものではありません。

日本版『ポケットモンスター 赤・青』の文章、名称、UI表記を基準に、Gen1Recomp上で当時の日本語版に近い体験を再現することを目標としています。

ROM由来の通常テキストだけでなく、Gen1Recomp側で直接生成される表示についても対応しています。

対象には以下のような経路が含まれます。

- `Strings()`
- `TextBox`
- `Font.draw`
- メニュータイトル／フッター
- Trainer Card
- Pokédex
- Fly
- Safari Zone
- Game Corner
- バトルHUD
- 状態異常表示
- その他Gen1Recomp固有UI

v0.5.5ではGen1Recomp 0.1.89の配布ランタイムを対象にBlue/shared表示経路を再監査し、その内容をv0.6.0にも引き継いでいます。

## スクリーンショット

### Pokémon Blue

#### オーキド博士との会話

![オーキド博士](screenshots/K89_BLUE_1.jpg)

#### 名前入力画面

![名前入力画面](screenshots/K89_BLUE_2.jpg)

#### ゲーム画面

![ゲーム画面](screenshots/K89_BLUE_3.jpg)

#### バトル画面

![バトル画面](screenshots/K89_BLUE_4.jpg)

Pokémon Redのスクリーンショットも順次追加します。

## インストール

配布用ZIPは **Releases** からダウンロードしてください。

1. Releasesから最新版の `K89-Pokemon-Gen1-JP-...zip` をダウンロードします。
2. ZIPを展開します。
3. `K89_POKEMON_RED_BLUE_JP` フォルダをGen1Recompの `mods` フォルダへ入れます。
4. Gen1Recompを起動します。
5. MOD一覧から **K89 Pokemon Red & Blue JP** を有効にします。
6. Pokémon RedまたはPokémon Blueを起動します。

> GitHub上部の **Code → Download ZIP** ではなく、Releasesにある配布用ZIPを使用してください。

## 対応環境

- Gen1Recomp 0.1.89+
- Pokémon Red
- Pokémon Blue

このMOD単体ではゲームを起動できません。

Gen1Recompと、ユーザー自身が用意した対応Pokémon ROMが必要です。

このリポジトリおよび配布ZIPにはROMは含まれていません。

## 不具合報告

未翻訳箇所、文字化け、表示位置の問題、クラッシュなどを発見した場合はGitHub Issuesから報告してください。

可能であれば以下を記載してください。

- Pokémon Red / Blueのどちらで発生したか
- スクリーンショット
- 発生場所
- 発生状況
- 再現手順
- 使用しているGen1Recompのバージョン

## 関連プロジェクト

### K89 Pokémon Gen2 JP

Pokémon Gold向けGeneration II日本語化MOD：

https://github.com/yaizoo/K89-Pokemon-Gen2-JP

現在はPokémon Goldに対応しています。Pokémon Silver / Crystalにはまだ対応していません。

## 開発支援

K89 Pokémon Gen1 JPは無料で公開しています。

開発、テスト、日本語化作業を支援していただける場合は、暗号資産での寄付を受け付けています。

寄付は完全に任意です。MODのダウンロードおよび利用に支払いは必要ありません。

**BTC**

`1P2xDJC99Jx4th5kXpwW1Jeg4uaw29Racm`

**ETH**

`0xa6d631b2984A0C1d93f3ADD828Ff204DC3272bF0`

**XMR**

`41sgKb1BLfz535b5bfspbQQB9RoeYzELDDNWraqAemsPcY32MXtQj1BXKb92pqmUTTBL3sEB29bRfd7xTN98e45rHjvDK9n`

**XRP**

`rDyA6b4FeEiAkVVhnos9QJReRxA1VgVsD7`

Destination Tag：不要

## 注意事項

このMODは非公式のファンプロジェクトです。

任天堂、株式会社ポケモン、ゲームフリーク、Creatures Inc.、その他の権利者とは関係ありません。

Pokémon、ポケットモンスター、および関連する名称・コンテンツの権利は、それぞれの権利者に帰属します。

このプロジェクトはROMを配布するものではありません。
