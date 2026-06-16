# GNU AGPL v3 License Cheatsheet

The **GNU Affero General Public License v3 (AGPL-3.0)** is the strongest copyleft license available. It extends the GPL's copyleft requirements to cover software accessed **over a network** — effectively closing the "SaaS loophole" where cloud providers could use GPL code without sharing their modifications.

## Quick Summary

| Property | Status |
| :--- | :---: |
| **Commercial Use** | ✅ Allowed (with full source disclosure) |
| **Modification** | ✅ Allowed |
| **Distribution** | ✅ Allowed |
| **Sublicensing** | ❌ Forbidden (must remain AGPL) |
| **Private/Internal Use** | ✅ Allowed (does not trigger copyleft) |
| **Must Disclose Source** | ✅ Yes — even for network/SaaS users |
| **Patent Grant** | ✅ Yes (explicit patent license from contributors) |

---

## The Defining Feature: Network Copyleft

AGPL-3.0 is specifically designed to close the **SaaS loophole** left by the GPL:

- Under the **GPL**, only users who *receive a copy* of the software can demand the source code. Cloud providers could run GPL software on their servers and never distribute binaries — so the copyleft was never triggered.
- Under the **AGPL**, if users interact with your software **over a network** (web browser, API, or any remote access), they have the right to receive the **complete corresponding source code**.

> **Practical impact**: If you build a SaaS product, web app, or cloud API using an AGPL library, you must publicly release your entire application's source code under AGPL-3.0.

---

## What You CAN Do

*   **Use commercially**: Run and sell the software — but you must open-source the entire stack.
*   **Modify**: Change, extend, and improve the codebase freely.
*   **Distribute**: Share the application with others along with its source code.
*   **Receive patent protection**: Contributors grant you an explicit, royalty-free patent license.

## What You MUST Do

*   **Disclose full source to network users**: If users interact with your modified AGPL software over a network, they are entitled to the complete source code. Provide a prominent link to download it.
*   **License the entire application as AGPL-3.0**: If your application incorporates AGPL code, the entire combined application must be licensed under AGPL-3.0.
*   **State all modifications**: Add prominent notices in modified files stating what you changed and when.
*   **Preserve license notices**: Keep all original copyright, license, and attribution notices intact.

## What You CANNOT Do

*   **Run a closed-source SaaS**: You cannot use AGPL code in a hosted service without releasing the full source code of your service.
*   **Relicense as proprietary or GPL-only**: You cannot change the license to something less restrictive.
*   **Hold authors liable**: The software comes with no warranty.

---

## AGPL vs GPL: What Is the Difference?

| | GPL-3.0 | AGPL-3.0 |
|---|---|---|
| Copyleft triggers on distribution | ✅ Yes | ✅ Yes |
| Copyleft triggers on network access | ❌ No (SaaS loophole) | ✅ Yes |
| Best for desktop/CLI tools | ✅ | — |
| Best for web services & APIs | — | ✅ |

---

## When to Choose AGPL-3.0

*   You build a web service and want to ensure all forks and SaaS deployments remain open source.
*   You want to offer a "open core" business model: free under AGPL, with a commercial license available for closed-source use.
*   Examples of AGPL software: MongoDB (pre-relicense), Plausible Analytics, Bitwarden (server-side), Gitea.
