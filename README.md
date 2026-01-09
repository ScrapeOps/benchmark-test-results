# ScrapeOps Benchmark Test Results

**Open Data Repository**

This repository contains the **raw test results** from ScrapeOps benchmark studies. All data is published for transparency, reproducibility, and independent analysis.

---

## Why Open Data?

We believe benchmark claims should be verifiable. By publishing raw outputs:

* Anyone can audit our methodology
* Researchers can perform alternative analyses
* Historical data enables trend tracking over time
* The community benefits from shared knowledge

---

## Available Benchmarks

| Benchmark | Description | Article |
|-----------|-------------|---------|
| [Proxy API Browser Fingerprinting](./Proxy%20API%20Browser%20Fingerprint%20Benchmark/) | Evaluates browser realism and anti-detection capabilities of proxy API providers | [Read Article](https://scrapeops.io/blog/scraping-tools-fingerprinting-benchmark/) |

---

## Repository Structure
Each benchmark folder contains:

* **README.md** — Overview of tests run, scope, and methodology
* **test-results.jsonl** — Unmodified test outputs in JSON Lines format

---

## Data Format

Results are stored as `.jsonl` (JSON Lines) — one JSON object per line. This format is:

* Easy to parse in any language
* Streamable for large datasets
* Git-friendly for diffs
* Compatible with pandas, jq, and common data tools

---

## Versioning

Benchmark runs are timestamped within the data files. When methodology changes significantly, we may create new benchmark folders to preserve historical comparability.

---

## Updates

| Date | Benchmark | Notes |
|------|-----------|-------|
| January 2026 | Proxy API Browser Fingerprinting | Initial release |

---

## Disclaimer

* Results reflect provider behavior **at the time of testing** only
* Configurations, APIs, and infrastructure evolve over time
* No provider was notified or given special treatment prior to testing
* We encourage providers to reach out if they believe results are inaccurate

---

## Links

* [ScrapeOps](https://scrapeops.io/)
* [ScrapeOps Blog](https://scrapeops.io/blog/)
* [ScrapeOps on GitHub](https://github.com/ScrapeOps)

---

## License

This data is provided for informational and research purposes. Please attribute ScrapeOps when using this data in publications or derivative works.
