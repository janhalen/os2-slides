# Gold Standard Infrastructure Pipelines – Opsummering

## Indholdsfortegnelse
1. Introduktion
2. Kerneprincipper for en god pipeline
3. Bronze-niveau (Fundamentals)
4. [Sølv-niveau (Kvalitet og Automatisering)](#sølv-niveau-kAvancerede forbedringer)
6. Fremtidige forbedringer
7. [ernebudskab

---

## Introduktion
- **Event:** London DevOps #87.1  
- **Speaker:** Nathan Webster  
- **Emne:** Hvordan man bygger en *gold standard* infrastruktur-pipeline.  
- **Motivation:** Infrastruktur-pipelines burde være en løst udfordring i 2025, men mange teams kæmper stadig.

---

## Kerneprincipper for en god pipeline
- **Automatiseret** – minimerer manuelle trin.
- **Driver kvalitet** – håndhæver standarder.
- **Friktionsfri for teams** – “thoughtless” oplevelse.

---

## Bronze-niveau (Fundamentals)
- **Branching-model:**  
  - Undgå Git Flow og long-lived branches.  
  - Brug **GitHub Flow** eller **Trunk-Based Development**.
- **Versionering:**  
  - Implementér **Semantic Versioning (SemVer)**.
- **Commits:**  
  - Brug **atomare commits** (én ændring pr. commit).  
  - Følg **Conventional Commits**-standarden.
- **Automatisering:**  
  - Brug **semantic-release** til versionsstyring, tagging og release notes.
- **CI/CD:**  
  - Moderne værktøjer som **GitHub Actions** (undgå Jenkins).  
  - Tilføj commit message checks.

---

## Sølv-niveau (Kvalitet og Automatisering)
- **Terraform-værktøjer:**  
  - `terraform fmt`, `validate`, `tflint`, **terraform-docs**.
- **Statisk kodeanalyse:**  
  - Brug **Checkov** til sikkerhed og compliance.
- **Shift-left:**  
  - IDE-plugins til auto-format og validering.  
  - **Pre-commit hooks** til lokale checks.
- **Deployment:**  
  - **Atlantis** til Terraform plan/apply via pull requests.

---

## Guld-niveau (Avancerede forbedringer)
- **TFM:** Nem styring af Terraform-versioner.
- **Danger:** Automatisér PR-checks og teamnormer.
- **Terraform Plan i PR:** Giver kontekst til reviewers.
- **Infracost:** Viser omkostningsændringer i PR.
- **Samlet pipeline:** Hurtig, robust, kvalitetssikret.

---

## Fremtidige forbedringer
- **LocalStack** til lokal AWS-test.
- **Unit tests for Terraform**.
- **Policy enforcement med OPA**.
- **Conventional Comments** til struktureret PR-feedback.

---

## Kernebudskab
En *gold standard* infrastruktur-pipeline er:
- **Hurtig, automatiseret, kvalitetssikret og omkostningsbevidst**.
- Bygget med værktøjer som:
  - **GitHub Actions, semantic-release, pre-commit, Checkov, Atlantis, Danger, Infracost**.

---

# Automatiserede Releases
Baseret på ensartet standard for arbejds og bidrags beskrivelser.

(commit og PR beskrivelser)

> Spar tid og skab det overblik der skal til for at forstå dit produkt.