# ⚡ RunSurge

> 🌐 *Distributed Peer-to-Peer Python Execution Framework*

RunSurge is a decentralized, peer-powered system that enables Python code to run across idle devices. It bridges the gap between users with  computational demands and contributors with spare resources — much like how Uber connects riders and car owners.

---

## 🧭 Table of Contents

- [📌 Overview](#overview)
- [✨ Key Features](#key-features)
- [🧱 System Architecture](#system-architecture)
- [🔧 Modules](#modules)
- [🎬 Demo](#demo)
- [⚙️ How It Works](#%EF%B8%8F-how-it-works)
- [👥 Contributors](#contributors)
- [📜 License](#license)

---

## 📌 Overview <a name="overview"></a>

💻 **RunSurge** lets users offload heavy Python workloads to a distributed network of contributors’ machines. Contributors are rewarded based on usage, while submitters get affordable, scalable compute power.

Inspired by the **collaborative economy**, RunSurge adopts the model of companies like Uber — turning idle computing resources into value.

---

## ✨ Key Features  <a name="key-features"></a>

- ⚙️ **Peer-to-Peer Architecture** — Worker nodes sync, share, and coordinate without central dependence.
- 🧠 **Static Code Analysis** — Transforms user code into safe parallel blocks using DDG + heuristics.
- 🧰 **Automatic + Manual Execution Modes** — Both automatic and manual parallelization supported.
- 🔐 **Code Security with Semgrep** — Filters unsafe shell, network, or file operations.
- 🔄 **Modular System Design** — Extendable to GPU, new scheduling rules, or third-party APIs.
- 📈 **Built-in Scheduler** — Optimizes task distribution based on estimated cost and memory.
- 🧪 **No Cloud Needed** — All components run on local or shared infrastructure.

---

## 🧱 System Architecture <a name="system-architecture"></a>

```plaintext
+------------------+       +-----------------------+       +------------------+
|   Code Submitter | <-->  |      Master Node      | <-->  |  Contributor Pool|
+------------------+       +-----------------------+       +------------------+

    - Schedules, monitors, aggregates   <->    - Executes tasks, syncs results
    - Parses code for parallel blocks         - Shares data peer-to-peer
```
![GP2](https://github.com/user-attachments/assets/9ad94b73-aa97-446e-ae4f-9f1f62c862ff)


---

## 🔧 Modules <a name="modules"></a>

### 🔹 Master Module
Coordinates distributed tasks, aggregates results, monitors failures, and ensures synchronization across worker nodes.

### 🔹 Worker Module
Accepts dispatched code, executes its assigned chunk, syncs results with peers, and reports completion.

### 🔹 Parallelization Module
Performs static AST and DDG-based analysis to extract code blocks that can be safely parallelized and estimates memory pressure per task.

---

## 🎬 Demo <a name="demo"></a>
https://drive.google.com/file/d/1pGlt4yIj4JC62GGIIM-A167wn34LlwDy/view?usp=sharing

---

---

## ⚙️ How It Works

1. 📝 User submits Python script.
2. 🔐 Script is Checked for Vulnerabilities.
3. 🧠 Static analysis breaks it into safe concurrent blocks.
4. 🚚 Tasks are scheduled across the network.
5. 🖥️ Contributors execute assigned tasks and sync data.
6. 🧩 Master collects results and returns final output.

---






## 👥 Contributors <a name="contributors"></a>

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/Omar-Said-4" target="_black">
        <img src="https://avatars.githubusercontent.com/u/87082462?v=4" alt="Omar Said"/>
        <br />
        <sub><b>Omar Said</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/MostafaMagdyy" target="_black">
        <img src="https://avatars.githubusercontent.com/u/97239596?v=4" alt="Mostafa Magdy"/>
        <br />
        <sub><b>Mostafa Magdy</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/nouraymanh" target="_black">
        <img src="https://avatars.githubusercontent.com/u/102790603?v=4" alt="Nour Ayman"/>
        <br />
        <sub><b>Nour Ayman</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/3abqreno" target="_black">
        <img src="https://avatars.githubusercontent.com/u/102177769?v=4" alt="Abdelrahman Mohamed"/>
        <br />
        <sub><b>Abdelrahman Mohamed</b></sub>
      </a>
    </td>
  </tr>
</table>


---

## 📜 License <a name="license"></a>

This project is licensed under the [MIT License](https://github.com/Run-Surge/.github/blob/main/LICENSE).
