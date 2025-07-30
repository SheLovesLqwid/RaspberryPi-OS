# 🍓 RaspberryPi-OS — Open Source ARM64 Operating System for Raspberry Pi & Education

> ⚠️ **Notice:** RaspberryPi-OS is actively in development and is **not yet production-ready**. It’s being built as a full-featured educational operating system for **Raspberry Pi hardware**, with plans for **future commercial deployment** in OS development courses and training programs.

![RaspberryPi-OS Banner](https://dummyimage.com/1000x300/111/fff&text=RaspberryPi-OS+-+Advanced+Educational+ARM64+Operating+System)

---

## 🧠 About RaspberryPi-OS

**RaspberryPi-OS** is a **64-bit ARM-based operating system kernel**, written in C and Assembly, tailored for the **Raspberry Pi platform** (AArch64 architecture). Unlike a “toy OS,” this project is being developed as a serious educational resource for **systems programming**, **low-level ARM architecture**, and **bare-metal development**.

It serves as the ARM64 companion to [LumaOS](https://github.com/SheLovesLqwid/LumaOS-x86-Educational-Kernel-Project), our x86-based learning kernel.

🔓 Open-source for now — 💼 Commercial course integration planned later SEE BOTTOM FOR MORE INFO!!!.

---

## 🌟 Why RaspberryPi-OS?

RaspberryPi-OS isn't a toy kernel — it's a **serious learning platform** built to eventually power:

* 🧑‍🎓 **In-depth systems programming courses** (online & in-class)
* 💻 **Full Raspberry Pi development curriculum**
* 🧩 A modular and hackable platform for ARM64 developers
* 🏫 Commercial educational licenses for schools, bootcamps, and online training platforms

---

## 🚀 Feature Overview

| Feature                          | Status  | Description                                                                 |
|----------------------------------|---------|-----------------------------------------------------------------------------|
| AArch64 Bare-Metal Bootloader    | ✅       | Fully custom booting process directly on Raspberry Pi hardware             |
| EL1 Stack Initialization         | ✅       | Initializes stack and kernel for Exception Level 1                         |
| UART Logging                     | ✅       | Serial port printing for debugging via UART0                               |
| MMU + Page Table Support         | ⏳       | Memory management unit and page translation (in progress)                 |
| Interrupt Handling               | ⏳       | ARM exception vectors and interrupt controller setup                       |
| GPIO + Timer Drivers             | ⏳       | Access to physical Raspberry Pi hardware (GPIO, Timer, etc.)               |
| Kernel Shell                     | ⏳       | Basic command-line shell over UART                                          |
| Scheduler                        | ⏳       | Multitasking framework for future userland support                         |
| Filesystem Integration           | ⏳       | VFS support with SD/MMC or ext2 planned                                    |

---

## 💻 Prerequisites

To build and run **RaspberryPi-OS**, ensure the following are installed:

- `aarch64-linux-gnu-gcc` (ARM64 cross-compiler)
- `make` (build system)
- `qemu-system-aarch64` (for emulated testing)
- Raspberry Pi 3B / 3B+ / 4 (for physical testing)
- Basic GNU/Linux dev environment

### 📦 Installation Example (Ubuntu/Debian)

```bash
sudo apt update
sudo apt install gcc-aarch64-linux-gnu make qemu-system-aarch64
```

---

## 🛠️ Getting Started

### 🔄 Clone the Repository

```bash
git clone https://github.com/SheLovesLqwid/RaspberryPi-OS.git
cd RaspberryPi-OS
```

### ▶️ Build and Run (QEMU Emulation)

```bash
make run
```

### 🧹 Clean the Build

```bash
make clean
```

---

## 💼 Commercial Vision

While RaspberryPi-OS is fully open-source today, the future roadmap includes:

* 🧑‍🏫 Structured course material for instructors
* 🧠 Project-based Raspberry Pi OS development curriculum
* 🧰 Developer SDK for embedded systems learning
* 🗂️ GUI-driven installer + file manager (future roadmap)
* 🧾 Optional enterprise classroom license + LMS integration

---

## 📜 License

**🛡️ GPL v3 — GNU General Public License, Version 3**

This project is licensed under the **GNU General Public License v3.0 (GPLv3)**. This means:

* 🔓 **Freedom to Use** — You are free to run this program for any purpose.
* 🛠️ **Freedom to Modify** — You can study the source code and make changes.
* 📤 **Freedom to Share** — You can redistribute the original or your modified version, under the same license.
* 💡 **Copyleft Clause** — Any derivative work must also be distributed under GPLv3 to ensure continued software freedom.

For complete legal details, see the full license text in [`LICENSE`](LICENSE) or visit: [https://www.gnu.org/licenses/gpl-3.0.html](https://www.gnu.org/licenses/gpl-3.0.html)

---

## 🏫 Educational Use & Commercial Roadmap

While **RaspberryPi-OS** is open-source under GPLv3, it is also the foundation of a **long-term educational and commercial initiative**:

* 🎓 **Open-source for learners and developers**: You’re free to fork, study, and build your own experiments.
* 🧑‍🏫 **Intended for future academic use**: A structured, course-ready edition will be launched for schools, bootcamps, and online learning platforms.
* 💼 **Commercial versions will expand the offering** with:

  * Rich documentation and video lectures
  * Integrated IDE & debugging tools
  * Certification-ready curriculum and exercises
  * Optional enterprise licenses for classroom and institutional use

These enhanced materials will coexist alongside the core open-source project, never restricting your right to learn, fork, or contribute under GPLv3.

---

## 🤝 Your Role in the Ecosystem

By contributing to RaspberryPi-OS, you support:

* 🔧 Better tools for teaching systems programming
* 📚 Free and open educational resources
* 🧪 A platform for ARM64 experimentation and innovation

Contributions remain GPLv3-licensed and help shape the foundation of future academic and enterprise editions.

---

## 🧩 Contributing

We welcome collaboration!

You can help by:

* Submitting pull requests
* Reporting issues or typos
* Writing hardware drivers or improving portability
* Expanding course-level documentation

To contribute, fork the repo and send a pull request or open an issue with your suggestion.

---

## ✨ Stay Connected

Want updates, dev logs, or to participate in the roadmap?

* 🧵 Discord Community: [Join us](https://discord.gg/eVQuBaMDvN)
* 📰 Dev Blog: *Coming soon*
* 🐦 Twitter / X: *Coming soon*

---

## 📚 Core Learning Resources

* [📖 Writing a Simple OS from Scratch (PDF)](https://www.cs.bham.ac.uk/~exr/lectures/opsys/10_11/lectures/os-dev.pdf)
* [🧠 JamesM's Kernel Dev Tutorials (Archived)](https://web.archive.org/web/20160412174753/http://www.jamesmolloy.co.uk/tutorial_html/index.html)
* [🌐 OSDev.org Wiki - Meaty Skeleton](https://wiki.osdev.org/Meaty_Skeleton)
* [🕹️ BrokenThorn OSDev Series](http://www.brokenthorn.com/Resources/OSDevIndex.html)
* [📘 The Little OS Book](https://littleosbook.github.io/)
* [💾 Dynamic Memory Allocation Explained](http://www.sunshine2k.de/articles/coding/cmemalloc/cmemory.html)

---

## 📈 SEO & Discoverability Keywords

```
RaspberryPi-OS, ARM64 operating system, AArch64 kernel, Raspberry Pi bare metal OS, Raspberry Pi custom OS, open-source kernel ARM64, write an OS for Raspberry Pi, system programming education, embedded kernel development, ARMv8 bootloader tutorial, QEMU Raspberry Pi OS, OS development ARM64, bare metal Raspberry Pi development, Raspberry Pi UART logging, Page table ARM64, GPIO driver Raspberry Pi, MIT licensed OS kernel, educational kernel for Raspberry Pi, systems programming teaching tool, C and ASM OS, memory management AArch64
```

---
