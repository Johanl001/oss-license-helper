# GNU GPL v2 License Cheatsheet

The **GNU General Public License version 2 (GPL-2.0)** is a strong copyleft license, first published by the Free Software Foundation in 1991. It is one of the most widely used open-source licenses in history, powering the **Linux kernel** and thousands of other foundational projects. While GPL-3.0 is the modern successor, GPL-2.0 remains critically relevant because many major projects explicitly use "GPL-2.0 only" and are *not* upgradeable to GPL-3.0.

## Quick Summary

| Property | Status |
| :--- | :---: |
| **Commercial Use** | ✅ Allowed (with full source disclosure) |
| **Modification** | ✅ Allowed |
| **Distribution** | ✅ Allowed |
| **Sublicensing** | ❌ Forbidden (must remain GPL-2.0) |
| **Private/Internal Use** | ✅ Allowed (no copyleft triggered) |
| **Must Disclose Source** | ✅ Yes, if distributed |
| **Patent Grant** | ❌ No explicit patent license in GPL-2.0 |

---

## The Viral (Copyleft) Clause

GPL-2.0's defining feature is its **reciprocal copyleft**:

*   If you distribute a binary or executable that **incorporates GPL-2.0 code**, you must provide the complete corresponding source code under the GPL-2.0.
*   **Private use** (internal tools, research, personal projects that are never distributed) does NOT trigger copyleft. Only distribution triggers it.
*   This "viral" nature means any project that integrates GPL-2.0 code and distributes it must itself be GPL-2.0 — even if you wrote the surrounding code yourself.

---

## What You CAN Do

*   **Use commercially**: Sell software that uses GPL-2.0 libraries, as long as you provide the full source code to buyers.
*   **Modify**: Change the source code and build upon it.
*   **Distribute**: Share the modified or unmodified software, along with its full source.
*   **Run privately**: Use GPL-2.0 software internally without any disclosure obligations.

## What You MUST Do

*   **Release the complete source code**: Anyone who receives your compiled program must be able to obtain the full, machine-readable source code. This can be done by including it with the binary or offering a written promise to supply it on request.
*   **State all modifications**: If you modified any GPL-2.0 files, add prominent notices in those files stating what changed and when.
*   **License under GPL-2.0**: All derivative works you distribute must also be licensed under GPL-2.0 (or, if the license says "GPL-2.0 or later", then GPL-3.0 is also an option).
*   **Preserve all notices**: Do not remove copyright notices, warranty disclaimers, or license headers from the source files.

## What You CANNOT Do

*   **Keep your source closed**: If you distribute a product containing GPL-2.0 code, you cannot keep your proprietary modifications secret.
*   **Sublicense**: You cannot add additional restrictions on top of the GPL-2.0 terms.
*   **Use patent retaliation protections**: GPL-2.0 does not include patent termination clauses (unlike GPL-3.0). This was a major driver of the upgrade to GPL-3.0.

---

## GPL-2.0 vs GPL-3.0: Key Differences

| Feature | GPL-2.0 | GPL-3.0 |
|---|---|---|
| Explicit patent grant | ❌ No | ✅ Yes |
| Anti-tivoization clause | ❌ No | ✅ Yes |
| Apache 2.0 compatible | ❌ No | ✅ Yes |
| DRM / Hardware lockdown | No restrictions | Prohibited for hardware shipping GPL code |
| "Or later" upgrade | Only if code says so | Available for new projects |

> The Linux kernel uses **GPL-2.0 only** (explicitly excluding "or later"), which means it can never be upgraded to GPL-3.0 without consent from all thousands of contributors.

---

## Apache 2.0 Incompatibility

One critical gotcha: **GPL-2.0 and Apache 2.0 are incompatible**. The Apache 2.0 license contains specific patent termination clauses that are considered additional restrictions under GPL-2.0, making the two licenses legally incompatible in the same binary. GPL-3.0 resolved this incompatibility explicitly.

---

## When to Choose GPL-2.0

*   You are contributing to an existing GPL-2.0 project (e.g., the Linux kernel) and must match its license.
*   You need legacy compatibility with a large ecosystem of GPL-2.0 software.
*   Examples: Linux Kernel, Git, MySQL (dual-licensed), GIMP, GCC (historically).
