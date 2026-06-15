# GPL License Cheatsheet (GPL-2.0 & GPL-3.0)

The **GNU General Public License (GPL)** is a strong copyleft license. It guarantees end users the freedom to run, study, share, and modify the software. Its most defining characteristic is the **reciprocal (viral) clause**: any derivative work of a GPL library must also be licensed under the GPL.

## Quick Summary

| Property | Status |
| :--- | :---: |
| **Commercial Use** | ✅ Allowed (with source code disclosure) |
| **Modification** | ✅ Allowed |
| **Distribution** | ✅ Allowed |
| **Sublicensing** | ❌ Forbidden (must remain GPL) |
| **Private/Internal Use** | ✅ Allowed (does not trigger copyleft) |
| **Must Disclose Source** | ✅ Yes, if distributed |
| **Patent Grant** | ✅ Yes (in GPL-3.0; GPL-2.0 does not contain it) |

---

## Key Differences: GPL-2.0 vs GPL-3.0

1.  **Patent Protection**: GPL-3.0 contains an explicit patent grant, meaning any contributor automatically grants you a license to any of their patents that cover their code.
2.  **Tivoization Loophole**: GPL-3.0 forbids "tivoization" (where hardware uses GPL code but refuses to run modified firmware, named after TiVo). Under GPL-3.0, you must provide installation instructions so users can run modified versions on the hardware.
3.  **License Compatibility**: GPL-3.0 is compatible with Apache 2.0; GPL-2.0 is not compatible with Apache 2.0.

---

## What You CAN Do

*   **Use commercially**: You can sell GPL software, but you must provide the source code to whoever buys it.
*   **Modify**: Change the source code to fit your needs.
*   **Distribute**: Share the software with others.

## What You MUST Do

*   **Open Source Your Code**: If you distribute a program that includes, links to, or is a modification of a GPL library, your entire program must be licensed under the GPL.
*   **State Changes**: If you modify GPL files, you must add prominent notices stating that you changed the files and the date of change.
*   **Provide Source Code**: You must make the full source code available to anyone who receives your binaries.

## What You CANNOT Do

*   **Close the Source**: You cannot bundle GPL code into a proprietary closed-source application and distribute it.
*   **Restrict Further Sharing**: You cannot add terms that restrict what recipients can do beyond what the GPL permits.

---

## When to Choose GPL

*   You want to ensure that any improvements made to your software by others are shared back with the community.
*   You want to prevent proprietary companies from repackaging your work as a closed-source product.
