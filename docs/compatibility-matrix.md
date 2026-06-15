# OSS License Compatibility Matrix

This document provides a comprehensive guide to understanding how open-source licenses interact with each other. It answers the question: *“Can I combine a library under License X with my project under License Y?”*

## Interactive Table Summary

In our interactive `index.html` tool, you can check compatibility directly. Below is the underlying compatibility logic between the most popular open-source licenses:

| Project License (Row) \ Library License (Col) | MIT / ISC | Apache 2.0 | MPL 2.0 | LGPL 2.1 | GPL 2.0 | GPL 3.0 | AGPL 3.0 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **MIT / ISC** | ✅ | ✅ | ⚠️ | ⚠️ | ❌ | ❌ | ❌ |
| **Apache 2.0** | ✅ | ✅ | ⚠️ | ⚠️ | ❌ | ❌ | ❌ |
| **MPL 2.0** | ✅ | ✅ | ✅ | ⚠️ | ❌ | ⚠️ | ❌ |
| **LGPL 2.1** | ✅ | ✅ | ⚠️ | ✅ | ❌ | ⚠️ | ❌ |
| **GPL 2.0** | ✅ | ✅ | ⚠️ | ✅ | ✅ | ❌ | ❌ |
| **GPL 3.0** | ✅ | ✅ | ⚠️ | ✅ | ❌ | ✅ | ❌ |
| **AGPL 3.0** | ✅ | ✅ | ⚠️ | ✅ | ❌ | ⚠️ | ✅ |

### Legend

*   **✅ Compatible**: You can merge or link this library into your project directly.
*   **⚠️ Conditions Apply**: Permitted under specific conditions (e.g., dynamic linking only, or keeping the library files separate).
*   **❌ Incompatible**: You cannot mix these licenses in the same project without violating one of them.

---

## Detailed Rules & Explanations

### 1. Permissive to Permissive (e.g., MIT, ISC, Apache 2.0)
Permissive licenses are universally compatible. You can include MIT or Apache 2.0 code in almost any project.
*   *Note on Apache 2.0*: It contains a patent grant clause. Combining Apache 2.0 code with GPL 2.0 projects is technically incompatible because GPL 2.0 has strict terms that don't support the specific patent conditions of Apache 2.0, whereas GPL 3.0 explicitly supports it.

### 2. Permissive Project containing Copyleft Library (e.g., MIT project using GPL library)
This is **incompatible**. If your project is licensed under a permissive license (like MIT) and you want to include/merge a GPL library, the GPL's "viral" clause triggers. Any derivative work containing GPL code must be licensed under the GPL as a whole, meaning you can no longer distribute it under a pure MIT license.

### 3. Copyleft Project containing Permissive Library (e.g., GPL project using MIT library)
This is **fully compatible**. Permissive licenses allow redistribution under any terms, including the GPL. You must retain the original copyright notice of the MIT/Apache library, but your overall project can remain GPL.

### 4. Weak Copyleft (e.g., LGPL 2.1, MPL 2.0)
*   **LGPL (Lesser GPL)**: Designed to allow linking from proprietary or permissive code. If you link the LGPL library *dynamically*, your project is compatible and does not need to be open-sourced. If you link it *statically*, you must provide the object code of your project so users can relink the library.
*   **MPL (Mozilla Public License)**: File-level copyleft. You can combine MPL files with permissive or proprietary files in a project, but any modifications to the *MPL files themselves* must be published under the MPL.

### 5. Strong Copyleft & Network Copyleft (e.g., GPL 3.0, AGPL 3.0)
*   **GPL (General Public License)**: Requires the entire distributed software to be open-sourced under the GPL.
*   **AGPL (Affero GPL)**: Closes the "SaaS loophole". If users interact with the software over a network (e.g., web app, cloud API), you must make the source code of the entire application available to them. You cannot combine AGPL code into a standard GPL project without upgrade provisions.
