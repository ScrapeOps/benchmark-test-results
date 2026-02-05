
# Stealth Browser Fingerprinting Benchmark

**Raw Test Results**

This folder contains the **raw fingerprinting test outputs** used in the ScrapeOps benchmark article:
[Stealth Browser Fingerprinting Benchmarks](https://scrapeops.io/proxy-providers/stealth-browser-fingerprint-benchmark/)

The purpose of this repository is **transparency**. These files are the source data behind all scores, tables, and conclusions.

---

## What’s Inside

Unmodified results captured during live testing, including:

* HTTP headers and Client Hints
* JavaScript-exposed browser properties
* Hardware, graphics, and device fingerprints
* Timezone, locale, and geo alignment signals
* Automation and headless detection flags
* Cross-session fingerprint entropy

No scoring or interpretation is performed here.

---

## Fingerprinting Tests Run

Each provider was evaluated across the following **15 browser fingerprinting tests**:

1. **Fingerprint Entropy Across Sessions**
   Detects repeated or deterministic fingerprints across runs.

2. **Header Realism**
   Validates modern browser header structure and formatting.

3. **Client Hints Coherence**
   Checks alignment between `sec-ch-ua*` headers and User-Agent.

4. **TLS / JA3 Fingerprint Realism**
   Verifies TLS signatures resemble real browsers, not backend libraries.

5. **Platform Consistency**
   Ensures OS reported in headers matches JavaScript platform values.

6. **Device-Type Coherence**
   Confirms viewport, touch points, and sensors match desktop or mobile claims.

7. **Hardware Realism**
   Evaluates CPU cores, memory, and GPU plausibility.

8. **Timezone vs IP Geolocation**
   Checks browser timezone alignment with proxy IP country.

9. **Language / Locale vs IP Region**
   Verifies browser language matches geographic expectations.

10. **Resolution & Pixel Density Realism**
    Detects unnatural or repeated screen resolutions.

11. **Viewport & Geometry Coherence**
    Flags impossible window and screen dimension combinations.

12. **Fonts & Plugins Environment**
    Assesses richness and OS-appropriate font and plugin lists.

13. **Peripherals Presence**
    Checks for microphones, speakers, and webcams typical of real devices.

14. **Graphics Fingerprints (Canvas & WebGL)**
    Validates execution-based graphics fingerprint outputs.

15. **Automation Signals**
    Detects WebDriver flags, CDP automation, and worker inconsistencies.

---

## Test Scope (Quick Overview)

* **Mode:** JavaScript rendering / browser mode
* **Locations:** United States, United Kingdom, Germany, Japan, Russia
* **Focus:** Stealth Browser APIs — browser realism, cross-layer consistency, automation leakage

Full methodology and scoring logic are explained in the article.

---

## How This Data Is Used

These results power:

* Provider comparison tables
* Fingerprint test matrices
* Benchmark scores and rankings
* Historical regression tracking

You are free to re-score or analyze the data independently.

---

## Updates

* Initial run: February 2026

Future benchmark runs will be versioned to preserve historical accuracy.

---

## Disclaimer

Results reflect provider behavior **at the time of testing** only.
Configurations, defaults, and infrastructure may change over time.

No provider was notified or tuned prior to testing.

---

## Links

* [Benchmark article](https://scrapeops.io/proxy-providers/stealth-browser-fingerprint-benchmark/)
* [ScrapeOps](https://scrapeops.io/)
* [ScrapeOps on GitHub](https://github.com/ScrapeOps)
