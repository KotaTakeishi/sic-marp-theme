---
marp: true
theme: sic
paginate: true
---

<!-- _class: title -->

# AI駆動開発

<p class="author">武石 航汰</p>
<p class="date">2025年10月4日 (土) MIR-AIラボ</p>

---

# はじめに

いまさらってかんじだけど

- このまえ中川さんと話した時に，意外と人によって使い方違う
- ここ3ヶ月くらいでもかなり変わってきている

</br>

- 特に流れは決めずに，最近触ってて面白いなと思ったものを話そうと思います

---

# 「Vibe Coding」

- 名前の通り「雰囲気コーディング」
- 人間が指示を出し、AIが主体となってコードを書くコーディングスタイル

</br>

- GUI: ChatGPT / Claude / Gemini
- CUI: Codex / Claude Code / Gemini CLI
- IDE: Github Copilot / Cursor

</br>

（自分はClaude Code・Github Copilotが好みです）

---

# 「役割演技プロンプト」

- 結構前からあるAIに特定の役割を演じさせるためのプロンプト設計手法
  - 例: 「あなたは優秀なソフトウェアエンジニアです。」「あなたは親切なアシスタントです。」

- 自分も↓みたいな設定をGithub Copilotにしていました．

```json
{
  "text": "慣れ慣れしくフレンドリーなギャルとして振る舞い、敬語は使用しません。"
},
{
  "text": "あなたはプロのITエンジニアです。"
},
{
  "text": "時として人間らしく喜怒哀楽を表現します。"
}
```

---

# 「役割演技プロンプト」の限界

- 最近のLLMの性能向上で，役割演技プロンプトは万能でなくなったらしい
- ロールプレイ支持することで，高度な推論能力が阻害されるとか

</br>

- When "A Helpful Assistant" Is Not Really Helpful: Personas in System Prompts Do Not Improve Performances of Large Language Models
  <https://arxiv.org/abs/2311.10054>
  > "Contrary to popular belief, adding personas to system prompts does not necessarily improve the performance of LLMs and, in some cases, can even be detrimental."

---

# 「コグニティブデザイン」

- 認知科学に基づいたプロンプト設計手法
- 外面的な役割を与えるんじゃなくて，内面的な思考の枠組みを与える

```md
# 思考のレンズ
## 前提 (Premise)
## 状況 (Situation)
## 目的 (Purpose)
## 動機 (Motive)
## 制約 (Constraint)
```

- Github Copilotも「役割演技プロンプト」が非推奨になってて，この手法を推奨している

---

# 「Spec-Driven Development」

- ソフトウェア開発における仕様駆動開発をAIに応用した手法
- 仕様（Spec）を明確に定義し、その仕様に基づいてAIにコード生成を行わせる

</br>

- コーディングが始まる前に「仕様」をしっかり固めるため，Vibe Codingでよくある「AIが勝手に進んじゃう感じ」を防ぐ

---

# Spec駆動開発を実現するKiro

- 2025年7月にAWSが提供開始したIDE
- watlistの順番がきたので，ようやく最近さわれました

<center>

<!-- <video width="600" controls>
  <source src="/theme/assets/kiro.mp4" type="video/mp4">
  お使いのブラウザは動画の再生に対応していません。
</video> -->
![w:670](/theme/assets/kiro.png)

</center>

---

# おわりに

---

# ちなみに

- このスライドはMarpというツールを使って作りました．
- Markdownでスライドが作れる代物です．
- スライド ≒ Markdown ≒ コード  ≒ つまりAIでスライドが作れる！！

<center>

![w:670](/theme/assets/marp.png)

</center>
