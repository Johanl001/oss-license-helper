# Creative Commons Zero (CC0) Cheatsheet

**Creative Commons Zero v1.0 (CC0-1.0)** is a **public domain dedication**, not a traditional license. By applying CC0 to your work, you waive all your copyright and related rights worldwide to the maximum extent permitted by law. The result is effectively placing your work in the **public domain** — anyone can use it for any purpose, anywhere, without any conditions.

## Quick Summary

| Property | Status |
| :--- | :---: |
| **Commercial Use** | ✅ Allowed |
| **Modification** | ✅ Allowed |
| **Distribution** | ✅ Allowed |
| **Sublicensing** | ✅ Allowed |
| **Private Use** | ✅ Allowed |
| **Must Disclose Source** | ❌ No |
| **Must Provide Attribution** | ❌ No — not required |
| **Patent Grant** | ❌ None explicit |

---

## What Makes CC0 Different

Unlike all other open-source licenses — which grant permissions while retaining copyright — CC0 **waives copyright entirely**:

*   There are **no conditions**. No attribution required. No license text to include.
*   The work is treated as if it were in the public domain, even in jurisdictions that do not recognize a direct "public domain" concept.
*   If the copyright waiver cannot be legally enforced in a given jurisdiction, CC0 includes a **fallback permissive license** that allows the same usage.

> This makes CC0 the most legally simple way to release software: recipients can do anything with the code, no strings attached.

---

## What You CAN Do (Everything)

*   **Use commercially**: Incorporate CC0 code into proprietary products with zero requirements.
*   **Modify**: Change, refactor, combine, translate, or transform the code in any way.
*   **Distribute**: Share with anyone, in any form, anywhere.
*   **Sublicense**: Release your project under any license you choose, including a proprietary one.
*   **Use without attribution**: You are not legally required to credit the original author.

## What You MUST Do

*   **Nothing.** There are no conditions in CC0.

## What You CANNOT Do

*   **Hold the author liable**: The "no warranty" clause still applies — CC0 waives copyright, not tort liability.
*   **Claim endorsement by the original author**: You cannot imply the original author endorses your product.

---

## CC0 and Software: A Note of Caution

CC0 is most commonly used for **data, datasets, images, documentation, and creative works**. For software code specifically, there are some nuances:

1.  **Patent rights**: CC0 explicitly does not waive patent rights. If the author holds a patent covering the software, CC0 does not grant you a patent license. For code where patent safety matters, Apache 2.0 is a safer permissive choice.
2.  **OSI status**: The OSI does not consider CC0 an approved open-source license for software (though Creative Commons licenses are common for content). This matters if you are publishing a library to a package registry that checks for OSI-approved licenses.

---

## CC0 vs MIT: Which Is More Permissive?

| | MIT | CC0 |
|---|---|---|
| Attribution required | ✅ Yes | ❌ No |
| License text required in distributions | ✅ Yes | ❌ No |
| Patent protections | ❌ No explicit grant | ❌ Explicitly excluded |
| OSI approved for software | ✅ Yes | ❌ No |

CC0 is the more permissive of the two — no conditions whatsoever.

---

## When to Choose CC0

*   You want your code, data, or creative work to be completely restriction-free — "take it and do anything."
*   You are releasing **datasets**, **reference implementations**, **training data**, or **example code** where attribution friction is undesirable.
*   You work in **government or public sector** and need to release work without any copyright encumbrances.
*   Examples: SQLite (public domain with a similar spirit), many datasets on Hugging Face, Wikimedia Commons media.
