# ISMI・Selete横断調査：資料一覧と確認範囲

調査日：2026-11-12（日本時間）
目的：装置オペレーションシナリオ・要求定義支援ツールの背景知識整理。
本資料は前回チャットに掲載した調査内容をファイルとして整理したもの。今回の作業はファイル化であり、追加調査・規格の再確認は行っていない。

## 1. 記載の区分

- ［資料記載］：取得した一次資料本文で確認した内容。
- ［規格関連・間接確認］：一次資料が説明するSEMI規格の概念。規格原本の直接確認ではない。
- ［分析］：本調査による比較・分類。
- ［設計示唆］：ツールへの検討提案。確定要求ではない。
- ［未確認］：本文未取得、原本との照合未了、確認範囲外。

「共通要素」は共有する概念・検討観点を指す。全装置へのFOUP、ロードポート、GEM300、EDAの実装要求を意味しない。
ページ番号は文書内の印刷ページを使用し、PDF通算ページとは区別する。

## 2. 対象資料

| ID | 資料名 | 版・発行情報 | 確認状況 |
| --- | --- | --- | --- |
| S1 | Equipment Data Acquisition (EDA) Version 0710 Guidance | ISMI、2010-11-30、#10115124A-ENG | 本文の関連箇所を確認。Cimetrix配布の原文PDF |
| S2 | 300 mm Operational Flowcharts and Scenarios, V.10 | ISMI、表題紙2004-04-30、#04014488A-TR | 本文の関連箇所を確認。ErgoTech配布の原文PDF |
| S3 | 300 mm Equipment Base Software Functionality Requirements – Fixed Buffer and Internal Buffer Type Equipment: Selete/International SEMATECH CIM Base Functionality Requirements Collaboration, Phase 1B | 当該本文の版・発行日は未確認 | 本文未取得。S4の参照情報まで確認 |
| S4 | 300 mm Equipment Base Software Functionality Requirements – Error Handling and Extended Scenarios: Selete/ISMT CIM Base Functionality Requirements Collaboration, Phase 2, Rev.2.0 | International SEMATECH、表題紙2001-12-21、#00114018B-XFR | JEITA-SMTJ公開PDFの本文を確認。図の細かな矢印・配置は未検証 |
| S5 | 製造装置オンライン機能要求仕様書分冊 通信シナリオ参考書〈内部バッファ／バッチ処理装置編〉 | 転載候補には第1.0版、2002-03-31と表示 | 原本PDF未取得。技術的結論の根拠に未採用 |
| S6 | ISMI Equipment Data Acquisition (EDA) Evaluation Method for the July 2010 Standards Freeze Level: Version 1.0 | ISMI、2011-07-31、#11065150A-ENG | 関連一次資料として§9.1～9.2を選択確認 |

### URL

- [S1 本文](https://www.cimetrix.com/hubfs/Equipment-Data-Acquisition-Guidance-document-0710.pdf)
- [S1 配布説明](https://www.cimetrix.com/eda-guidance-document-download)
- [S2 本文](https://www.ergotech.com/files/guides/ISMI%20Operational%20Flows%20and%20Scenarios.pdf)
- [S3 旧参照先（前回アクセス不可）](http://www.sematech.org/public/docubase/document/3953cxfr.pdf)
- [S4 本文](https://www.jeita-smtj.com/jp/pdf/Selete/Selete%EF%BC%88%E6%97%A7%29/%E3%83%A9%E3%82%A4%E3%83%B3%E7%94%9F%E7%94%A3%E5%8A%B9%E7%8E%87%E5%90%91%E4%B8%8A/ISMI%E5%8D%94%E6%A5%AD%E8%A3%BD%E9%80%A0%E8%A3%85%E7%BD%AE%E9%96%A2%E4%BF%82/Selete%EF%BD%A5ISMT%20300mm%E8%A3%BD%E9%80%A0%E8%A3%85%E7%BD%AE%E3%82%BD%E3%83%95%E3%83%88%E3%82%A6%E3%82%A8%E3%82%A2%E5%9F%BA%E6%9C%AC%E6%A9%9F%E8%83%BD%E8%A6%81%E6%B1%82%E4%BB%95%E6%A7%98%E6%9B%B8%28Phase2%E8%8B%B1%E8%AA%9E%E7%89%88%29.pdf)
- [S5 第三者転載候補1](https://happylibus.com/doc/727993/製造装置オンライン機能要求仕様書分冊-通信シナリオ参考書)
- [S5 第三者転載候補2](https://paperzz.com/doc/6583118/製造装置オンライン機能要求仕様書分冊-通信シナリオ参考書)
- [S6 本文](https://www.cimetrix.com/hubfs/ISMI-EDA-Evaluation-Method-document.pdf)

S1・S2・S6は発行主体自身のサイトではなく、表題紙・発行主体・識別子を確認できる一次資料の配布コピーとして使用した。検索結果の掲載日・クロール日を発行日として扱っていない。

## 3. 調査観点と主要参照箇所

| 観点 | 出典 |
| --- | --- |
| 装置階層・分解粒度 | EDA Guidance（S1）§3.1.1 pp.11–12、§3.2.4 pp.18–20 |
| MaterialLocation・所在 | EDA Guidance（S1）§3.2.6 pp.20–21、§3.4.2 pp.47–50 |
| キャリア・ロット・基板・ジョブ | EDA Guidance（S1）§3.3.3 p.31、§3.4.1 pp.45–47、Phase 2（S4）§3.1 p.5 |
| 状態・事象・遷移 | EDA Guidance（S1）§3.3.3 pp.30–38、Operational Flowcharts（S2）§4.2.6～4.2.7 pp.82–84 |
| 責任分担 | Operational Flowcharts（S2）§3.2 p.19、Phase 2（S4）§4.1～4.2 pp.34–35 |
| 正常・異常・復旧 | Operational Flowcharts（S2）§2.1 p.2、§4.2 pp.75–90、Phase 2（S4）§4 pp.34–65 |
| 類型差 | EDA Guidance（S1）§3.4.4 pp.51–54、Phase 2（S4）§4.4～4.5 pp.42–48 |

## 4. 適用上の注意

［資料記載］

- S1は0710 EDAの補足指針。要求と推奨を区別している。出典：S1 §1.1～1.2 p.1、§1.6.1 p.3。
- S2は工場・装置に該当する部分を選択して使う資料。出典：S2 §1 p.1。
- S4は代表構成・代表異常を扱い、全装置・全要求を網羅しない。出典：S4 §2.1 p.2、§4.1 pp.34–35。

［分析］

- S1の「shall」を、そのまま要求定義ツールの必須仕様にしない。
- S2・S4の代表例を、すべての装置に共通する運用へ一般化しない。
- SEMI原本の条文・全属性・全遷移・現行版への適合性は未確認。

## 5. 未取得・版の問題

- Phase 1B本文は未取得。S4 §2.3.1 p.3は3953cxfr.pdfを参照する一方、S2 §1.1 p.1は00053953D-XFRを参照する。対応・差分は未確認。
- 日本語参考書は転載候補のみ。原本の章・ページは未確認。
- S2は表題紙、改訂履歴、参照規格で基準版の表現が異なる。表題紙、改訂履歴p.vi、§1.1 p.1を別々に保持する。
- S1 §3.4 p.45が参照するCommon Metadata配布物は未取得。

未取得は「存在しない」「公開されていない」という断定ではない。
