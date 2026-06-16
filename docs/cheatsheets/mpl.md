# Mozilla Public License 2.0 Cheatsheet

The **Mozilla Public License 2.0 (MPL-2.0)** is a **weak (file-level) copyleft** license, sitting between fully permissive licenses (MIT, Apache) and strong copyleft licenses (GPL, AGPL). It was designed by Mozilla to allow maximum commercial flexibility while still ensuring that improvements to MPL-licensed files are shared back.

## Quick Summary

| Property | Status |
| :--- | :---: |
| **Commercial Use** | ✅ Allowed |
| **Modification** | ✅ Allowed |
| **Distribution** | ✅ Allowed |
| **Sublicensing** | ⚠️ MPL files must stay MPL; your own code can use any license |
| **Private Use** | ✅ Allowed |
| **Must Disclose Source** | ⚠️ Only for modified MPL files |
| **Patent Grant** | ✅ Yes, explicit patent license from contributors |

---

## The Key Feature: File-Level Copyleft

The MPL's copyleft is scoped to **individual files**, not the whole project:

*   If you **modify a file** that was originally MPL-licensed, you must publish the source of that modified file under the MPL.
*   Files **you create yourself** that are added to the project can use any license you choose — including a proprietary one.
*   Your **overall application** does not need to be open-sourced, even if it uses MPL components.

This makes MPL-2.0 a popular choice for library authors who want to allow proprietary use while ensuring that direct improvements flow back to the community.

---

## What You CAN Do

*   **Build proprietary applications**: Combine MPL code with your own closed-source code — as long as MPL files remain separate and are published under MPL.
*   **Use commercially**: No restrictions on commercial use.
*   **Distribute binaries**: Ship your application without releasing your proprietary code.
*   **Receive patent protection**: Contributors explicitly grant you a royalty-free patent license to run the code.

## What You MUST Do

*   **Publish modifications to MPL files**: If you change any `.js`, `.py`, or other file originally under the MPL, you must publish the modified source of *that file* under the MPL.
*   **Keep files separate**: Do not combine MPL source code with your own code into the same file, or the copyleft spreads to the combined file.
*   **Include the license and copyright**: Every distribution must include the MPL-2.0 license text and original copyright notices.
*   **Notify recipients**: Anyone who receives the software must know which files are under MPL-2.0 and how to obtain the source for those files.

## What You CANNOT Do

*   **Use author trademarks**: You cannot use the original project's logos or brand to endorse your product.
*   **Hold contributors liable**: The software is provided without warranty.
*   **Remove the MPL notice from existing files**: You cannot convert MPL files to a different license without the original copyright holder's permission.

---

## How MPL Compares to Other Licenses

| | MIT | MPL-2.0 | GPL-3.0 |
|---|---|---|---|
| Proprietary apps allowed | ✅ | ✅ | ❌ |
| Copyleft scope | None | File-level | Whole project |
| Modifications must be shared | ❌ | ✅ (file level) | ✅ (full project) |
| Patent grant | ❌ | ✅ | ✅ |

---

## When to Choose MPL-2.0

*   You want your library to be usable by commercial projects but still want improvements to come back.
*   You are building a library where "file-level" reciprocity is sufficient.
*   Examples of MPL-2.0 software: Firefox, Thunderbird, LibreOffice (parts), HashiCorp Vault (pre-BSL change).
