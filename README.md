# Jordan Del Pilar 👋

Backend & Platform Automation Engineer. Building resilient middleware, IaC, and containerized workflows.

📄 <b>Resume:</b> <a href="https://resume.delpilar.net" target="_blank">Resume (PDF)</a>  
📧 **Email:** jordan@delpilar.net  
📍 **Location:** Lemoore, CA  

---

### 🛠️ Tech Stack & Tooling

* **Languages:** Python (FastAPI, Pytest, Pydantic), Go (Working Knowledge), Bash
* **Infrastructure & Ops:** Ansible, Podman (Rootless/Quadlets), Docker, Linux (Ubuntu)
* **CI/CD:** GitHub Actions, Gitea Actions
* **Cloud & Security:** GCP, Secret Manager, HMAC-SHA1
* **Tooling & Backups:** Restic, Traefik, AdGuard Home, Gitea, Ntfy

---

### ⚙️ Featured Projects

#### [johto-infra](https://github.com/redjordan2539/johto-infra)
Ansible configuration-as-code managing my homelab using Podman Quadlets.
* Configured automated SFTP backups via restic and systemd timers.
* Automated CI/CD pipelines via Gitea Actions.
* Primary repository hosted on my [self-hosted Gitea](https://git.delpilar.net/jdelpilar/johto-infra) instance; GitHub is a downstream mirror.

#### [Chiron-Relay](https://github.com/redjordan2539/Chiron-Relay)
FastAPI webhook relay for Twilio SMS.
* Uses Pydantic for validation and FastAPI background tasks for async processing.
* HMAC-SHA1 request verification and GCP Secret Manager integration.
* Containerized with Docker (`USER app`) and tested with Pytest.

#### [sundown](https://github.com/redjordan2539/sundown)
Go daemon for calculating solar times and sending alerts.
* Zero third-party dependencies.
* Atomic file writes (`.tmp` to `rename`) for state persistence.
* Structured logging via `log/slog` and posts directly to ntfy.
