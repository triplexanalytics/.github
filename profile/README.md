## Triplex Analytics

We build local-first data privacy tooling. Mask a real table, generate a synthetic one that
behaves like it, and score how risky a dataset is to share, all without the data leaving your
machine, your CI or your browser tab.

There is no server, no upload and no telemetry. Datasets, identifiers, mapping files and
credentials stay where you run the tool.

### Triplex

[**triplex**](https://github.com/triplexanalytics/triplex) is the open-source core (Apache-2.0):
one Rust engine with Arrow-compatible data contracts, delivered as a command-line tool, a Docker
image, a WebAssembly web UI, Python bindings and a Jupyter widget.

| Product | What it does |
|---|---|
| **SchemaCast** | Schema inference, `.triplex.yaml` contracts, validation and format conversion |
| **Anonymizer** | Pseudonymization with a separate mapping file, and synthetic data that keeps the dependencies between columns |
| **DatasetCard** | Privacy-risk scoring per dataset, column and record (k-anonymity, l-diversity, t-closeness) |
| **DriftGuard** | Schema-regression and statistical-drift checks between a baseline and a candidate, built for CI |
| **ModelCard** | Fairness and slice metrics for a binary classifier |

```sh
cargo install triplex          # command-line tool
pip install triplexanalytics   # Python bindings
```

**Triplex Pro** is the paid extension of the web UI, adding synthetic data generation and
sketch-based synthesis in the browser.

### About us

Triplex Analytics was founded in 2021 as a data consultancy for municipal governments, work we
still do today. Our team includes data experts with PhD degrees, and our director is an
associate professor of Visual Data Science at Utrecht University.

### Links

- Website and documentation: [triplexanalytics.io](https://triplexanalytics.io)
- Live demo on synthetic data: [demo.triplexanalytics.io](https://demo.triplexanalytics.io/)
- Contact: [info@triplexanalytics.io](mailto:info@triplexanalytics.io)
- Security reports: see [SECURITY.md](https://github.com/triplexanalytics/triplex/blob/main/SECURITY.md)
