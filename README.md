# MedAgent

**Agent-as-a-Service for clinical intake and evidence support.**

MedAgent collects history, retrieves clinical evidence, triages risk, and prepares a clinician handoff without replacing medical judgment.

面向医疗问诊的 Agent：完成病史采集、临床证据检索和风险分诊，并准备医生交接，不替代医疗判断。

**Status:** Project scaffold · [Portfolio](https://0x0addc001.github.io/#use-cases)

**Important:** This repository is not a medical device and must not be used for diagnosis or treatment without qualified clinical oversight.

## Agent loop

| Stage | Responsibility |
|---|---|
| Data | EHR, guidelines, intake dialogues, red-flag rules |
| Models | Medical LLM, clinical retrieval, risk classifier |
| Training | Clinical dialogue SFT, safety preference optimization |
| Inference | Streaming intake, evidence retrieval, triage |
| Harness | EHR, scheduling, escalation and clinician-review tools |
| Eval | Clinical safety, triage accuracy, hallucination, bias |

## Initial scope

- Use deterministic red-flag escalation rules.
- Cite clinical sources for every evidence-based statement.
- Keep a clinician in the loop for all consequential decisions.

## Roadmap

- [ ] Clinical safety taxonomy
- [ ] Synthetic intake evaluation set
- [ ] Retrieval-grounded intake flow
- [ ] Clinician handoff report
- [ ] Human evaluation protocol

## Engineering principles

- Safety overrides helpfulness.
- State uncertainty explicitly.
- Never collect or expose more health data than necessary.

