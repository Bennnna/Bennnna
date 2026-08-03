<p align="center">
  <a href="https://github.com/Bennnna/Phymargin_coc">
    <img src="https://raw.githubusercontent.com/Bennnna/Phymargin_coc/main/docs/assets/physmargin-cover.svg" width="100%" alt="PhysMargin-CoC cover" />
  </a>
</p>

<h1 align="center">Hi, I'm Jiwoo Jung</h1>

<p align="center">
  AI researcher working on multimodal reasoning, autonomous-driving intelligence, and evidence-grounded model evaluation.
</p>

<p align="center">
  <a href="https://github.com/Bennnna/Phymargin_coc"><img src="https://img.shields.io/badge/Flagship-PhysMargin--CoC-0f766e?style=for-the-badge" alt="PhysMargin-CoC" /></a>
  <a href="mailto:xhfl99@dgu.ac.kr"><img src="https://img.shields.io/badge/Email-Dongguk_University-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/jiwoo00"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
</p>

---

## PhysMargin-CoC

My current flagship research project is **Physical-Margin Chain-of-Contradiction Auditing for Reasoning–Physics Consistency in Vision-Language-Action Models for Autonomous Driving**.

Multimodal driving models may produce fluent action-oriented explanations that remain incompatible with independently computed physical evidence. PhysMargin-CoC audits that mismatch through an inspectable external pipeline:

```text
WOMD state at t = 45
  -> BEV RGB + leakage-controlled observation text
  -> Base / DoRA multimodal reasoning
  -> 12 driving predicates

Independent state path
  -> TTC, headway, braking, RSS, comfort, action-compliance margins
  -> applicability masks

Predicates + margins + frozen 12 x 6 relation
  -> pairwise contradiction evidence
  -> traceable offline diagnosis
```

<p align="center">
  <a href="https://github.com/Bennnna/Phymargin_coc"><b>Explore the PhysMargin-CoC repository →</b></a>
</p>

---

## Research Focus

- **Vision-Language-Action reasoning** for autonomous-driving scenes
- **Reasoning–physics consistency** rather than linguistic plausibility alone
- **Deterministic external auditing** with no trainable auditor parameters
- **Physical and behavioral margins** with text-independent applicability
- **Parameter-efficient adaptation** through paired Base/DoRA evaluation
- **Reproducible experimentation** with immutable artifacts and claim-to-evidence mapping

---

## What the Project Contributes

| Component | Role |
|---|---|
| Multimodal input | WOMD-derived BEV image plus leakage-controlled current-state text |
| Reasoning model | Paired Base and DoRA-adapted multimodal generation |
| Predicate layer | Twelve action-oriented driving claims with confidence and evidence spans |
| Margin layer | TTC, headway, braking, RSS-style, comfort, and action-compliance residuals |
| Applicability | Geometry- and state-derived masking independent of generated language |
| Auditor | Frozen predicate–margin relations and attributed pairwise evidence |
| Reproducibility | Split, model, checkpoint, metric, figure, and checksum manifests |

PhysMargin-CoC is designed for **offline, traceable model auditing**. It is not presented as a vehicle controller, crash predictor, or operational safety guarantee.

---

## Technical Stack

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch" />
  <img src="https://img.shields.io/badge/Transformers-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" alt="Transformers" />
  <img src="https://img.shields.io/badge/PEFT-7C3AED?style=for-the-badge" alt="PEFT" />
  <img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white" alt="CUDA" />
  <img src="https://img.shields.io/badge/WOMD-2563EB?style=for-the-badge" alt="WOMD" />
</p>

---

## Current Research Standard

- No result is reported before the corresponding run, metric recomputation, leakage audit, and checksum verification pass.
- Operational contradiction labels are not described as accident or real-world safety ground truth.
- Planned figures and tables remain explicitly marked until generated from archived artifacts.
- Unsupported safety, publication, and performance claims are excluded from public documentation.

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Bennnna&show_icons=true&theme=tokyonight&hide_border=true" height="165" alt="GitHub stats" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Bennnna&color=0f766e&style=flat-square&label=Profile+Views" alt="Profile views" />
</p>

<p align="center"><i>Building inspectable multimodal systems whose reasoning can be checked against the physical state they describe.</i></p>
