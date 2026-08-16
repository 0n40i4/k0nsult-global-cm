# CLAIMS.md — public claim register (k0nsult-global-cm)

Generated from [`k0nsult-tools/docs/CLAIMS-TEMPLATE.md`](https://github.com/0n40i4/k0nsult-tools/blob/master/docs/CLAIMS-TEMPLATE.md)
(OSS-0-06).

| id | statement | class | proof_ref / roadmap_ref | repo_status_ref | verified_at |
|---|---|---|---|---|---|
| `clm-0001` | This repo ships two static HTML surfaces for the Cameroon node of the global-expansion track (PL + EN). | DOWOD | `ls surfaces/` → `ai-truth-kamerun.html`, `ai-truth-kamerun-en.html` present | — | 2026-08-02 |
| `clm-0002` | This track is separate from the EU track by design, kept apart from `k0nsult-eu-shield` so the EU sovereignty scope is not diluted, with its own funding/support track (no EU-earmarked resources). | NARRACJA | — (an organisational/funding-governance statement about resource allocation; not something this repo's own files can independently prove — it describes a decision made elsewhere) | — | 2026-08-02 |
| `clm-0003` | `/api/*` calls (if any) are the integration boundary; the k0nsult.cloud engine is proprietary and not in this repository. | NARRACJA | — (negative/scope claim, true by omission of engine code — not independently provable from this repo alone) | — | 2026-08-02 |
| `clm-0004` | This repo does not claim any K0NSULT pilot, deployment, or government adoption in Cameroon — unlike `k0nsult-global-ar` (Argentina), this repo's README does not contain an equivalent explicit "no pilot" disclaimer sentence. | GAP | Checked: `grep -in "pilot\|adopted\|adoption" README.md` returns no match in this repo's README, unlike `k0nsult-global-ar/README.md`:7-10 which states this explicitly. Flagged as a documentation gap worth closing (same disclaimer pattern used consistently would strengthen claim<=proof posture here too) — not remediated in this task (out of the stated PLIKI scope for OSS-2-07, which is CLAIMS.md only). | — | 2026-08-02 |
| `clm-0005` | This repo's proposed `x-k0nsult.status` leans toward a controlled-research-equivalent value, not a live deployment. | GAP | `../k0nsult-eu-shield/generator.config.yml` records `status: CONTROLLED_RESEARCH` for this repo (OSS-1-07 proposed `RESEARCH_LAYER`, not in the canonical enum — see `OSS-0-01`); writing any status into `publiccode.yml` is Fala 1, WYMAGA_ACK: TAK — not yet applied | `k0nsult-global-cm#x-k0nsult.status` | 2026-08-02 |

## Placeholder row (copy for new claims)

| id | statement | class | proof_ref / roadmap_ref | repo_status_ref | verified_at |
|---|---|---|---|---|---|
| `clm-00NN` | *(exact claim text)* | *(DOWOD\|GAP\|NARRACJA)* | *(ref, or "—" if NARRACJA)* | *(optional, or "—")* | *(YYYY-MM-DD)* |

| clm-0006 | GAP | `publiccode.yml` (x-k0nsult.manifest.hash / sbom.hash) wskazuje na hash `sbom.json` sprzed regeneracji w tym PR — po merge będzie niezgodny mimo deklaracji `evidence_class: DOWOD`. Generator `gen-publiccode.mjs` nie istnieje w żadnym dostępnym repo (sprawdzone: to repo, k0nsult-tools) — nie da się przeliczyć bez fabrykacji. Wymaga ręcznej naprawy przez kogoś z dostępem do generatora, albo świadomego obniżenia evidence_class do czasu naprawy. | recenzja Fala 4, 2026-08-16 |
