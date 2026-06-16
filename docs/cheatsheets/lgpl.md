# GNU LGPL v2.1 License Cheatsheet

The **GNU Lesser General Public License v2.1 (LGPL-2.1)** is a **weak copyleft** license designed specifically for shared libraries. It allows proprietary applications to link against LGPL libraries without triggering the full GPL copyleft, making it the go-to license for open-source library authors who want broad adoption without requiring commercial users to open-source their applications.

## Quick Summary

| Property | Status |
| :--- | :---: |
| **Commercial Use** | ✅ Allowed |
| **Modification** | ✅ Allowed |
| **Distribution** | ✅ Allowed |
| **Sublicensing** | ❌ Not permitted (must remain LGPL) |
| **Private Use** | ✅ Allowed |
| **Must Disclose Source** | ⚠️ Only if you modify the library itself |
| **Dynamic Linking (App stays proprietary)** | ✅ Yes |
| **Static Linking (App stays proprietary)** | ⚠️ Requires object file sharing |
| **Patent Grant** | ❌ Not explicitly included in LGPL-2.1 |

---

## The Key Feature: The Linking Exception

The LGPL was created to allow the GPL's copyleft to apply *only to the library itself*, not to the application that uses it:

*   **Dynamic Linking** (`.dll`, `.so`, `.dylib`): If your application links to an LGPL library at runtime (dynamically), **your application can remain entirely closed-source**. No source disclosure is triggered.
*   **Static Linking** (compiled into your binary): If you compile the LGPL library directly into your application binary, you must provide the compiled **object files** of your application so that users can relink the library with a modified version. You do not need to release your full source code, but sharing object files may expose proprietary code.
*   **Modification of the library**: If you modify the LGPL library's own source code, those modifications must be released under the LGPL.

> **Bottom line**: For most developers, using an LGPL library dynamically (the default for most languages and build systems) is completely hassle-free.

---

## What You CAN Do

*   **Use in proprietary software**: Link to LGPL libraries from a closed-source commercial application.
*   **Use commercially**: No restrictions on commercial exploitation.
*   **Modify the library**: Change the LGPL library's source code as needed.
*   **Distribute your application**: Ship your closed-source application with the LGPL library (as a separate dynamic file).

## What You MUST Do

*   **Release library modifications**: If you make changes to the LGPL library itself, you must release those changes under the LGPL.
*   **Allow users to re-link**: Users must be able to swap out the LGPL library for a different version. Provide your application's object files (`.o`, `.obj`) if you statically link.
*   **Provide or point to the library source**: Include a copy of the library's source code or provide a written offer to supply it.
*   **Keep all copyright and license notices**: Do not remove LGPL notices from the library files.

## What You CANNOT Do

*   **Hold developers liable**: No warranty is provided.
*   **Prevent users from modifying the library**: You cannot take steps (such as DRM) to prevent users from installing a modified version of the LGPL library.
*   **Sublicense to closed terms**: The library itself cannot be relicensed as proprietary.

---

## LGPL-2.1 vs LGPL-3.0

| | LGPL-2.1 | LGPL-3.0 |
|---|---|---|
| Anti-tivoization clause | ❌ | ✅ (inherited from GPL-3.0) |
| Apache 2.0 compatible | ❌ | ✅ |
| Most common for libraries | ✅ | Less common |

Most major open-source libraries (glibc, Qt, FFmpeg) use LGPL-2.1.

---

## When to Choose LGPL-2.1

*   You maintain a library and want it to be usable in proprietary software (unlike GPL).
*   You want improvements to the library itself to remain open-source.
*   Examples: glibc (GNU C Library), Qt (LGPL option), FFmpeg (LGPL parts), CUPS.
