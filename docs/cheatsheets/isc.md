# ISC License Cheatsheet

The **ISC License** is an extremely simple, permissive open-source license. It is functionally identical to the MIT License and the 2-Clause BSD License, just with even shorter and cleaner legal wording. The ISC License is the default license of the OpenBSD project and is widely used in the Node.js/npm ecosystem.

## Quick Summary

| Property | Status |
| :--- | :---: |
| **Commercial Use** | ✅ Allowed |
| **Modification** | ✅ Allowed |
| **Distribution** | ✅ Allowed |
| **Sublicensing** | ✅ Allowed |
| **Private Use** | ✅ Allowed |
| **Must Disclose Source** | ❌ No |
| **Must Share Modifications** | ❌ No |
| **Patent Grant** | ❌ None explicit |

---

## Why ISC Exists

The ISC License was created by the **Internet Systems Consortium** (the organization behind BIND, ISC DHCP, and other core internet infrastructure) to provide a clean, legally sound permissive license. Older permissive licenses (like the original 4-Clause BSD) contained clauses that were redundant or created practical problems (like the "advertising clause"). The ISC License strips all of that away to a bare minimum.

---

## The Entire ISC License Text

The ISC License is so short it fits in a paragraph:

```
Copyright (c) [Year] [Copyright Holder]

Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
```

---

## What You CAN Do

*   **Use commercially**: Use ISC-licensed code in proprietary, closed-source software.
*   **Modify freely**: Refactor, extend, or rewrite the code without restriction.
*   **Distribute**: Package and ship the code with your software.
*   **Sublicense**: Include ISC code in a project under a different license (even proprietary).

## What You MUST Do

*   **Include the copyright notice and the ISC license text**: In all copies or substantial portions of the software, you must include the original copyright line and the permission notice. This is the only requirement.

## What You CANNOT Do

*   **Hold the author liable**: The software is provided "as is" without any warranty. You cannot sue the author if it causes problems.

---

## ISC vs MIT: What Is the Difference?

Functionally, **there is no meaningful difference**. Both are permissive, both require attribution, neither requires sharing source. The OSI officially considers them functionally equivalent.

The ISC License is considered slightly preferable by some lawyers because:
- The MIT License contains outdated language inherited from older templates.
- The ISC License is cleaner and avoids the ambiguous phrase *"without limitation"* found in some MIT variants.

---

## When to Choose ISC

*   You want maximum simplicity — the shortest possible compliant open-source license.
*   You are publishing a small npm package and want zero friction for users.
*   Examples of ISC-licensed software: OpenBSD, many npm core packages (e.g., `semver`, `glob`, `isexe`).
