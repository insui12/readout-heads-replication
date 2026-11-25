# Answer-Selective Donor Patching of Readout Heads under Matched Injection Magnitude in Long-Context Retrieval

Seojin Choi and Geunseok Yang (corresponding author: gsyang@hknu.ac.kr)
Department of Computer Science and Engineering, Hankyong National University

Replication files for the manuscript.

| File | Content | SHA-256 |
|---|---|---|
| `readout_heads_manuscript.pdf` | Manuscript | `a7ad44cfee9e59fd49c2c652c0d7a3634006fe63530369dfea8ab222b2b98357` |
| `readout_heads_supplement.pdf` | Supplementary material | `6dda5b54168935589cf7105fae507b1f3d3e5f6d25a466cb8cb4e58d2462a3b7` |
| `readout_heads_replication.zip` | Replication package: code, registration files, stored records and paper values ([release asset](https://github.com/insui12/readout-heads-replication/releases/tag/v1.3)) | `689e2ff205662fd077fa8d61cd08c5f193ccd57c8cfc479ab3a9017f6db32d45` |
| `readout_heads_latex_source.zip` | LaTeX source of the manuscript and the supplementary material | `361717f6e64dbe8d9ed1b50d24c299baf68c9927ea93f4fa31e262ff4c219e2b` |

The replication package (224 MB) is attached to release `v1.3`, the release that the manuscript cites, and archived at https://doi.org/10.5281/zenodo.24527973.
Check a download with `sha256sum <file>`.

## Reproduce

Requires Linux x86-64 and Python 3.12. Inside the unpacked `package/` directory of the replication package:

```
python3.12 -m venv .venv
.venv/bin/python -m pip install --no-index --find-links reproduction_env/wheels numpy==2.2.6
PYTHON="$PWD/.venv/bin/python" bash reproduce.sh
```

Installation uses the bundled NumPy wheel; the reproduction runs offline, loads no model, takes about eleven minutes and about 4 GiB of memory, and ends with `REPRODUCTION OK`.
It recomputes the confirmation and sensitivity reports of both studies and the reports of the analyses added outside the registration from the stored records, and regenerates the result macros, tables and data files of the manuscript; summaries of the development stages, the power simulations and the reviews are stored inputs.
`package/README.md` describes the contents, the registration files and what is withheld.

## Licence

Authors' own code: Apache-2.0. Authors' own data and documents: CC BY 4.0. Full texts are in `LICENSE`.
Third-party material keeps its upstream licence and attribution, listed in `package/LICENSES/` of the replication package; the LaTeX class and style files carry their own licence.
