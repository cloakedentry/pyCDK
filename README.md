🐍 pyCDK - Python Container Defense Toolkit

**pyCDK** is a Python-based offensive security toolkit tailored for auditing, exploiting, and interacting with containerized environments such as Kubernetes clusters and Docker containers. Inspired by CDK (Container Exploitation Toolkit), this toolset replicates many of its capabilities using Python, making it easier to customize and extend.

---

## 🔥 Features

### 🎯 Evaluation
- Full security posture analysis inside containerized environments
- Detects sensitive environment variables, dangerous Linux capabilities, and privileged containers
- Deep risk scoring for paths, kernel configs, processes, and more
- Summary of HIGH/MEDIUM/LOW severity issues for instant insights

### 🔍 Discovery & Enumeration
- Dump K8s secrets, RBAC, configmaps, service accounts
- Show all pods, capabilities, mounts, network interfaces, etc.
- Map Kubernetes services and endpoints
- Perform local path severity audits

### 💥 Exploitation Modules
- Run known container escapes and lateral movement techniques
- Reverse shell generators, docker.sock exploits, host escape POCs
- Easily list and execute exploits with `python main.py run --list`

### 🛠️ Tooling Suite
- Netcat-style TCP tunneling with `nc`
- Query Kubernetes API with `kcurl`
- Query Docker sockets with `ucurl`
- Inspect etcd with `ectl`
- Process listing (`ps`), network info (`ifconfig`), and more

---

## 🚀 Quick Start

```bash
git clone https://github.com/yourname/py-cdk.git
cd py-cdk
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

python main.py --help
