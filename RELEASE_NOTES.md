# Release Notes

## V0.3 — Initial Bilingual Public Release

- **Release date:** September 1, 2026
- **Author:** Wei Roy Wang
- **Project:** HyperUnit Network
- **GitHub:** [@aspttwwly](https://github.com/aspttwwly)
- **Copyright:** © 2026 Wei Roy Wang. All rights reserved.

### Included Artifacts

- Chinese white paper, content version `v1.2`.
- English white paper, content version `v1.2`.
- Chinese interactive companion demo, version `V0.3`.
- English interactive companion demo, version `V0.3`.

Release downloads use portable ASCII filenames with explicit `EN` and `ZH-CN` language tags. Their content is identical to the corresponding repository artifacts; use `RELEASE_ASSET_SHA256SUMS.txt` to verify downloaded assets.

The companion demo applies the white paper's minimum closed loop to pre-publication validation of weekly bank account balances. It uses synthetic data to make Responsibility, typed Inputs, Dependency Snapshot, Claim, human Decision, simulated Reality Fact, and Evidence visible in one portable example.

### Validation Completed

- Both Word files are valid DOCX containers with no macros, comments, or tracked revisions.
- Both Word files link to the corresponding same-directory HTML demo.
- All nine images in each Word file include title and description alternative text.
- Both HTML files contain valid embedded JSON and JavaScript.
- Both HTML files retain a restrictive Content Security Policy and contain no network or persistent-storage API calls.
- The English HTML contains no Chinese characters and links back to the English Word white paper.
- Desktop and 375-pixel mobile regression checks found no horizontal overflow.
- All four synthetic scenarios, human Decision gating, Reality validation, local layout demonstration, and authoring controls passed browser regression.
- Browser console warning/error count was zero during regression.

### Important Boundaries

- The Manifest is a non-normative public example and does not grant permissions.
- The demo uses synthetic data only and performs no real business execution.
- The HTML carrier is not a substitute for Runtime governance, Persistence, Registry, security controls, or enterprise systems.
- Protocol fields and implementation conformance remain subject to the planned Core Protocol Specification.
- Public access does not grant an open-source license or redistribution permission.

### Version Map

- Release package: `V0.3`
- White paper content: `v1.2`
- Companion demos: `V0.3`
- Example Manifest: `0.1-draft`, non-normative
- Example Capability: `prepublish-check@0.1.0`
