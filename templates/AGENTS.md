# AGENTS.md — Research repository working agreement

> **模板**：请按实际项目修改。Codex 会读取适用的 `AGENTS.md`；本文件不意味着授予新的训练、提交或远程推送权限。

## Context

- Project: `[项目名称]`.
- Read `docs/research_status.md` and relevant entries in `docs/experiment_log.md` before important research tasks.
- Inspect only the code, configurations, results and logs relevant to the current task.
- Preserve the research question and evaluation protocol; never invent missing evidence.

## Roles

- ChatGPT 00: research questions, hypotheses, novelty, priorities and experiment briefs.
- ChatGPT 01: independent literature, protocol, statistical and evidence review.
- Codex: implementation, testing, training/evaluation when authorized, technical risk checks and factual documentation.
- User: final approval of major research decisions, high compute budgets and irreversible actions.

## Evidence and experiments

- Prefer executed code, frozen configs, logs and original results over narrative summaries.
- Distinguish idea / implemented / executed / development result / independent confirmation.
- Check subject/sample split isolation, target access, tuning budget, metric code and comparisons.
- Record negative experiments; obey predeclared Go/No-Go gates; do not tune around a failed stop rule without a new user-approved protocol.
- Do not reclassify old experiments under a new protocol after the fact.

## Documentation

- `docs/research_status.md`: current state, verified conclusions, open risks and next steps.
- `docs/experiment_log.md`: append-only-style history; experiment ID, dates, inputs, splits, seeds, configs, metrics, result paths and limitations.
- Make corrections explicitly, preserving the historical record.

## Safety / Git

- Never upload restricted participant or patient data, raw signals, credentials, large checkpoints or proprietary assets without explicit permission and data-use review.
- Preserve existing modifications; no destructive Git operations, data cleanup or overwriting reliable artifacts without approval.
- Check `.gitignore`, tracked files and Git history before first push.
- Local documentation edits do **not** automatically update GitHub. Only commit/push under current user authorization.
- Do not start training when only asked to audit or prepare documentation.

## Communication

- State what was completed, verified, blocked and not done.
- Escalate missing scientific or protocol decisions; make routine reversible engineering decisions directly.
- Return concise evidence paths, experiment IDs and Git state, not unsupported success claims.
