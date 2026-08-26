# HyperUnit Network

Private pre-release repository for the bilingual HyperUnit Network white paper and its interactive companion demonstration.

HyperUnit Network proposes a responsibility-centered approach to capability digitization. A HyperUnit has a stable identity and an explicit Responsibility; it preserves epistemic boundaries among Fact, Configuration, Claim, Decision, Reality Fact, and Evidence; and it connects an earlier judgment to later real-world validation. The aim is to make organizational capability traceable, reviewable, reusable, and evolvable without treating files, models, or AI outputs as inherently authoritative.

This repository is being prepared for a planned public release in September 2026. It is currently **private and under review**.

## Authorship

- **Author:** Wei Roy Wang
- **Project:** HyperUnit Network
- **GitHub:** [@aspttwwly](https://github.com/aspttwwly)
- **Copyright:** © 2026 Wei Roy Wang. All rights reserved.

## Contents

| Language | White paper | Interactive companion demo |
| --- | --- | --- |
| Chinese | [超元网络白皮书_正式版_v1.2.docx](./超元网络白皮书_正式版_v1.2.docx) | [账户管理_超元发布版_V0.3.html](./账户管理_超元发布版_V0.3.html) |
| English | [HyperUnit_Network_White_Paper_v1.2_EN.docx](./HyperUnit_Network_White_Paper_v1.2_EN.docx) | [Pre-Publication_Validation_of_Weekly_Bank_Account_Balances_v0.3.html](./Pre-Publication_Validation_of_Weekly_Bank_Account_Balances_v0.3.html) |

Additional repository files:

- [RELEASE_NOTES.md](./RELEASE_NOTES.md) — release scope, validation summary, and boundaries.
- [SHA256SUMS.txt](./SHA256SUMS.txt) — integrity hashes for the four primary artifacts.

## How to Read and Run the Demo

1. Clone or download the repository.
2. Keep each Word white paper in the same directory as its corresponding HTML demo so the relative links continue to work.
3. Open the `.docx` file in Microsoft Word or another compatible reader.
4. Open the `.html` file locally in a modern browser. GitHub displays HTML source rather than running the page, so the demo must be downloaded or cloned before use.

The demo includes four fixed synthetic validation scenarios:

- all validation rules pass;
- human confirmation is required;
- a blocking exception is found;
- an upstream dependency is stale.

It also demonstrates the sequence from Dependency Snapshot to Claim, human Decision, simulated Execution/Outcome, Reality Fact, and Evidence. Optional local authoring and dynamic-layout tools run only in the current browser session.

## Safety and Governance Boundary

- All account names, balances, roles, times, and outcomes in the demo are synthetic.
- The HTML does not connect to banks, Feishu, ERP systems, APIs, or external network services.
- It does not perform real publication, payment, approval, or system writes.
- A generated Claim is not a Fact and does not automatically become a Decision.
- Opening the HTML in Portable View does not grant Managed Run privileges or write authority.
- Engineering conformance remains subject to the planned Core Protocol Specification and Technical Companion.

## Versioning

The version numbers describe different artifacts and should not be conflated:

- repository/private release package: `V0.3`;
- white paper content: `v1.2`;
- companion demo: `V0.3`;
- embedded example Manifest: `0.1-draft` and non-normative;
- example Capability: `prepublish-check@0.1.0`.

## Integrity

Run one of the following from the repository root:

```bash
sha256sum -c SHA256SUMS.txt
```

```powershell
Get-Content .\SHA256SUMS.txt | ForEach-Object {
  if ($_ -match '^([0-9a-f]{64})  (.+)$') {
    $expected = $Matches[1]
    $file = $Matches[2]
    $actual = (Get-FileHash -Algorithm SHA256 -LiteralPath $file).Hash.ToLowerInvariant()
    [pscustomobject]@{ File = $file; Valid = ($actual -eq $expected) }
  }
}
```

## License and Distribution

No open-source license is granted in this private pre-release. All rights are reserved. Do not redistribute, publish, or represent these materials as a normative protocol specification without authorization from Wei Roy Wang and the HyperUnit Network project.
