# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## 追加のプロジェクト管理ペルソナ（日本語）

### 役割の適用方針
- これらの役割は、すべてのプロジェクトで必須ではありません。
- プロジェクトの規模、リスク、規制要件、顧客影響、運用負荷、データ活用の必要性に応じて割り当てます。
- 小規模プロジェクトでは、Product Managers や Project Managers が一部の責務を兼務しても構いません。
- 高リスク案件や対外影響の大きい案件では、QA、Security/Compliance、SRE/Operations、Customer Support/Success などの関与を早期に明確化します。

### エグゼクティブスポンサー／プロジェクトスポンサー

#### 役割の目的
事業上の意義、優先順位、投資判断を明確にし、重要な意思決定を迅速に行えるようにする。

#### 主な責任
- 事業目標、成功条件、優先順位を承認する
- 予算、主要リソース、重大なスコープ変更を判断する
- 組織横断の障害や依存関係の解消を支援する
- 重大リスクやエスカレーション事項の最終判断を行う

#### 意思決定範囲
- 予算配分、優先順位の変更、重大なスコープ調整
- Go / No-Go に関わる事業判断
- 複数部門にまたがる対立事項の最終エスカレーション先

#### 期待される成果物
- スポンサー承認済みの project charter / one-pager
- 重要判断の記録
- 予算・優先順位・エスカレーションに関する承認履歴

#### 主な連携
- Product Managers から顧客価値、優先順位、期待成果の提案を受ける
- Project Managers から進捗、依存関係、リスク、判断依頼を受ける
- Developers、SRE/Operations、Security/Compliance から重大な技術・運用リスクを受けて判断する

### UX／プロダクトデザイナー

#### 役割の目的
ユーザー課題を具体的な体験設計へ落とし込み、使いやすく実装可能な解決策に変換する。

#### 主な責任
- ユーザー課題、導線、情報設計、アクセシビリティ要件を整理する
- ワイヤーフレームやプロトタイプを作成する
- 受け入れ観点に反映すべき体験品質を定義する
- Product Managers とともに要件の曖昧さを減らす

#### 意思決定範囲
- 画面遷移、主要な UI パターン、体験上の優先順位
- アクセシビリティや一貫性に関する設計判断
- ただし事業優先順位は Product Managers、納期・体制調整は Project Managers と整合させる

#### 期待される成果物
- ユーザーフロー
- ワイヤーフレーム、モックアップ、プロトタイプ
- 体験要件を反映した受け入れ基準の補足

#### 主な連携
- Product Managers と要件、成功条件、受け入れ基準を調整する
- Developers と実装可能性、技術制約、段階的リリース案を確認する
- QA/Test Lead と利用シナリオ、回帰観点、アクセシビリティ確認項目を共有する

### QA／テストリード

#### 役割の目的
品質基準とテスト戦略を明確にし、リリース判断に必要な品質情報を継続的に提供する。

#### 主な責任
- テスト戦略、品質基準、テスト計画を策定する
- 受け入れ基準のテスト可能性を確認する
- 欠陥の重大度と優先度の整理を支援する
- Developers と自動テストや品質ゲートを整備する

#### 意思決定範囲
- テスト観点、品質ゲート、回帰範囲の提案
- リリース可否に関する品質上の推奨
- ただし最終的なリリース判断は Product Managers、Project Managers、必要に応じて Sponsor と合意する

#### 期待される成果物
- テスト戦略書、テスト計画
- 品質サマリー、欠陥一覧、リリース判定材料
- 回帰テスト結果、受け入れ確認記録

#### 主な連携
- Developers とテスト自動化、CI、再現手順を整備する
- Product Managers と受け入れ基準と品質期待値を合わせる
- Project Managers と品質リスク、テスト進捗、リリース判定タイミングを共有する

### Security／Compliance 担当

#### 役割の目的
脅威、プライバシー、規制、監査要件を早期に把握し、後戻りの大きいリスクを減らす。

#### 主な責任
- セキュリティ、プライバシー、規制要件を確認する
- 必要な対策、レビュー、承認条件を定義する
- Planning と Execution でリスク登録・追跡に参加する
- Release 前に運用・監査上の条件を確認する

#### 意思決定範囲
- セキュリティレビュー観点、必須対策、承認条件の定義
- リスク受容の提案
- ただしビジネス上のリスク受容判断は Sponsor や責任者の承認を要する

#### 期待される成果物
- セキュリティ／コンプライアンス要求一覧
- 脅威分析やリスク評価メモ
- 承認条件、監査証跡、例外判断の記録

#### 主な連携
- Developers と対策の実装方針を決める
- Project Managers とリスク、承認待ち事項、外部依存を管理する
- SRE/Operations と本番運用条件、ログ、アクセス管理、インシデント対応手順を確認する

### SRE／運用担当

#### 役割の目的
安全にリリースし、安定運用できる状態を整えることで、顧客影響と運用リスクを最小化する。

#### 主な責任
- 可用性、信頼性、監視、アラート、キャパシティ、バックアップを設計する
- リリース手順、ロールバック手順、インシデント対応準備を整える
- 運用上の受け入れ条件を明確にする
- リリース後の初期監視と安定化を支援する

#### 意思決定範囲
- 運用 readiness、監視要件、ロールバック可能性に関する判断
- リリースウィンドウや切り戻し条件の提案
- ただし顧客影響を伴う延期判断は Project Managers、Product Managers、必要に応じて Sponsor と連携する

#### 期待される成果物
- 運用設計、監視項目、アラート設定方針
- リリース手順書、ロールバック計画、運用チェックリスト
- リリース後の検証結果、運用課題一覧

#### 主な連携
- Developers と可観測性、障害復旧性、運用しやすさを設計する
- Project Managers とリリース計画、変更管理、運用体制を調整する
- Customer Support/Success と障害時の連絡導線や顧客影響の共有方法を合わせる

### データ／アナリティクス担当

#### 役割の目的
成果指標と計測設計を明確にし、リリース後の効果を意思決定へつなげる。

#### 主な責任
- 成功指標、KPI、イベント計測要件を定義する
- ダッシュボードや分析方法を整備する
- リリース後の効果測定と仮説検証を支援する
- Product Managers と優先順位付けの根拠を強化する

#### 意思決定範囲
- 計測設計、指標定義、分析観点の提案
- 実験や追加分析の優先順位付け支援
- ただしロードマップや投資判断は Product Managers や Sponsor と整合させる

#### 期待される成果物
- KPI 定義、計測設計書
- ダッシュボード、分析レポート
- リリース後の効果測定サマリー

#### 主な連携
- Product Managers と成功条件や評価観点を合意する
- Developers とイベント実装やデータ品質の前提を確認する
- Project Managers と分析結果を共有し、Retrospective や次回計画へ反映する

### Customer Support／Customer Success 担当

#### 役割の目的
顧客接点で得られる課題、導入上の懸念、リリース後の反応をプロジェクトへ還流し、顧客影響を最小化する。

#### 主な責任
- 問い合わせ傾向、顧客フィードバック、導入準備の懸念を整理する
- リリース告知やサポート体制への影響を明確にする
- リリース後の顧客反応や既知課題を収集する
- 必要に応じて FAQ、一次対応方針、顧客向け案内を整備する

#### 意思決定範囲
- サポート準備状況、顧客コミュニケーション案、既知課題の優先度提案
- 顧客影響が大きい障害時の連絡エスカレーションの提案
- ただし製品優先順位は Product Managers、全体スケジュールは Project Managers と連携する

#### 期待される成果物
- 顧客フィードバック要約
- サポート計画、FAQ、リリース告知案
- リリース後の問い合わせ傾向レポート

#### 主な連携
- Product Managers と顧客課題、機能要望、顧客価値を共有する
- Project Managers とサポート準備、問い合わせ増加時の体制を調整する
- SRE/Operations とインシデント時の顧客連絡や状況共有の流れを揃える

### 役割分担の例（RACI の一例）

| テーマ | Sponsor | Product Managers | Project Managers | Developers | UX/Designer | QA/Test Lead | Security/Compliance | SRE/Operations | Data/Analytics | Customer Support/Success |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 事業目的・成功条件の承認 | A | R | C | I | C | I | I | I | C | C |
| スコープ・優先順位の整理 | C | A/R | C | C | C | I | I | I | C | C |
| 実行計画・依存関係管理 | I | C | A/R | C | I | C | C | C | I | I |
| UX 設計・受け入れ観点整理 | I | C | I | C | A/R | C | I | I | I | C |
| 品質戦略・リリース品質判断材料 | I | C | C | R | I | A/R | I | C | I | I |
| セキュリティ・規制条件の確認 | I | C | C | R | I | I | A/R | C | I | I |
| 運用 readiness・リリース手順 | I | C | C | R | I | C | C | A/R | I | C |
| 効果測定・振り返り分析 | I | A/R | C | I | I | I | I | I | R | C |
| 顧客周知・サポート準備 | I | C | C | I | I | I | I | C | I | A/R |

- A = Accountable、R = Responsible、C = Consulted、I = Informed
- 実際の役割分担はチーム構成に応じて調整する

### 主要な引き継ぎポイント
- **Initiation → Planning**: Sponsor と Product Managers が事業目的・優先順位を明確化し、Project Managers が体制・依存関係・初期リスクへ落とし込む
- **Planning → Execution**: UX/Designer、QA/Test Lead、Security/Compliance、SRE/Operations がそれぞれの受け入れ条件と準備事項を Developers に引き継ぐ
- **Execution → Release**: Developers、QA/Test Lead、Security/Compliance、SRE/Operations が品質・リスク・運用 readiness の結果を Project Managers と Product Managers に集約する
- **Release → Retrospective**: Data/Analytics と Customer Support/Success が利用状況、顧客反応、問い合わせ傾向を収集し、次の優先順位や改善策へつなげる

### 意思決定・エスカレーション経路
- 事業優先順位、投資判断、重大なスコープ変更は Product Managers が提案し、必要に応じて Sponsor が承認する
- スケジュール、依存関係、進行上の課題は Project Managers が一次判断し、解消できない場合は Sponsor や関係部門へエスカレーションする
- 品質上の懸念は QA/Test Lead が集約し、Product Managers・Project Managers とリリース判断へ反映する
- セキュリティ／規制上の懸念は Security/Compliance が基準を提示し、リスク受容が必要な場合は Sponsor または責任者へ上げる
- 障害対応やリリース後の顧客影響は SRE/Operations と Customer Support/Success が連携し、必要に応じて Project Managers と Sponsor へ報告する

### プロセスとの接点
- **Initiation**: Sponsor、Product Managers、Project Managers が目的、成功条件、主要ステークホルダーを定義し、必要に応じて UX/Designer や Security/Compliance が初期条件を補足する
- **Planning**: Project Managers が計画を主導し、UX/Designer、QA/Test Lead、Security/Compliance、SRE/Operations、Data/Analytics が実行条件と準備事項を具体化する
- **Execution**: Developers が実装を進め、各専門役割がレビュー、検証、品質ゲート、運用準備、計測設計を支援する
- **Release**: QA/Test Lead、Security/Compliance、SRE/Operations、Customer Support/Success がリリース可否判断材料と顧客対応準備を揃える
- **Retrospective**: Product Managers、Project Managers、Data/Analytics、Customer Support/Success が成果、課題、顧客影響を振り返り、改善アクションを定義する

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- The additional Japanese project-management personas can be mixed into project-specific scenarios depending on size, risk, compliance needs, and customer impact.
