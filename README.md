# README

**KuVuln** is an automated security bot designed to audit, secure, and monitor your entire repository. From Kubernetes manifests to application dependencies and container images, KuVuln acts as a tireless digital sentry, ensuring that security is never an afterthought.

---

## 🚀 Overview

KuVuln solves the "Security Gap" in DevSecOps by automating deep-dive analysis on every push and pull request. It doesn't just scan; it orchestrates the best security engines in the industry to provide a unified risk report directly in your GitHub UI.

### 🧩 Core Capabilities

* **☸️ Kubernetes Hardening:** Audits manifests, Helm charts, and Kustomize files against NSA-CISA hardening guides and CIS Benchmarks.
* **📦 Deep SCA (Software Composition Analysis):** Scans `npm`, `pip`, `go`, `cargo`, and `maven` for known CVEs (Common Vulnerabilities and Exposures).
* **🐳 Container Shield:** Deep-scans Dockerfiles for insecure instructions (e.g., `root` execution) and base image vulnerabilities.
* **🔑 Secret Guardian:** Analyzes full git history to detect leaked API keys, tokens, and private certificates.
* **📊 Native GitHub Integration:** Pushes results directly to the **Security Tab** via SARIF, enabling line-by-line code annotations.

---

## 🛠️ Zero-Installation Setup

KuVuln is designed to run entirely in the cloud. No local setup required.

- **Workflow Setup**: Copy the kuvuln-full.yml file into your .github/workflows/ directory.

- **Configuration**: Add kuvuln-config.json to your root directory to set your security thresholds.

- **Activation**: Commit the files. KuVuln will automatically trigger on the next push or pull_request.

## 🛡️ Powered By

KuVuln orchestrates a suite of elite open-source security engines:

- Trivy: Advanced vulnerability and misconfiguration scanner.
- Gitleaks: High-fidelity secret detection in git history.
- Semgrep: Static analysis for application logic and patterns.

## 📜 License
Licensed under the Apache License, Version 2.0 (the "License"). You may obtain a copy of the License at:

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

## 🤝 Contributing
We welcome security researchers and developers to join the KuVuln mission!

1. Fork the repo.
2. Create your feature branch.
3. Submit a Pull Request.

**Built with precision for the cloud-native era.**
