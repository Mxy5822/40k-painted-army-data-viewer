# 40K Painted Army Value Scorecard v2026 - eBay Data Scraper and Viewer

> A browser-based Warhammer 40,000 tool for collecting live painted army listings from eBay, evaluating their value with MSRP and a paint premium, and publishing cleaned JSON and JS data in the 2026 format.

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/dylanwnipscott3878/40k-painted-army-data-viewer?style=flat-square)](https://github.com/dylanwnipscott3878/40k-painted-army-data-viewer)

---

<p align="center">
  <a href="https://dylanwnipscott3878.github.io/40k-painted-army-data-viewer/">
    <img src="https://img.shields.io/badge/Download-40K%20Painted%20Army%20Value%20Scorecard%20Latest-brightgreen?style=for-the-badge" alt="Download 40K Painted Army Value Scorecard">
  </a>
</p>

> **[Download 40K Painted Army Value Scorecard v2026](https://dylanwnipscott3878.github.io/40k-painted-army-data-viewer/)**

---

[Download Latest Build](https://dylanwnipscott3878.github.io/40k-painted-army-data-viewer/)

---

## What This Project Does

40K Painted Army Value Scorecard turns painted Warhammer 40,000 army listings into a structured comparison dataset. It retrieves current eBay listings, applies a scoring model based on MSRP and an added paint premium, and generates cleaned files for viewing or further processing.

The project is intended for comparing painted army offers across factions without manually working through unstructured search results. Its output includes a standalone HTML scorecard as well as JSON and JS data files, allowing the collected information to be viewed, filtered, sorted, or integrated into other workflows.

---

## Capabilities

- Collects live painted army listings from eBay
- Calculates listing value with an MSRP plus paint premium model
- Writes cleaned JSON for downstream processing
- Creates JS data output that can be loaded directly by the web viewer
- Provides a standalone HTML interface with sorting and filtering
- Includes coverage for all factions, including the Chaos and Be'lakor edition
- Focuses on comparing the value of Warhammer 40,000 armies
- Converts raw listing results into a more practical review format

---

## Getting Started

Clone the repository or obtain the project files, then run the scraper and export process before opening the generated viewer.

1. Clone the repo:
   `git clone https://github.com/dylanwnipscott3878/40k-painted-army-data-viewer.git
2. Change into the project directory:
   `cd 40k-armies-scorecard-scraper`
3. Run the scraper or build process for your local environment
4. Launch the generated HTML viewer and provide the exported data files

For the published build, use the download link above and open the included viewer in your browser.

---

## Workflow

The normal process is:

1. Collect painted army listings by running the eBay scraper
2. Build the cleaned JSON and JS data exports
3. Open the standalone scorecard viewer
4. Sort, filter, and compare the resulting scored listings
5. Examine faction results, including available Chaos and Be'lakor entries

A local review cycle can look like this:

- Update the scraped listing data
- Recalculate the score output
- Open the viewer to examine the highest-ranked results
- Reuse or export the generated files in other tools

---

## Settings

Configuration is generally handled by the scraper and export pipeline. A setup may use values similar to the following:

```json
{
  "source": "eBay",
  "score_model": "MSRP + paint premium",
  "output": ["json", "js"],
  "viewer": "standalone HTML",
  "coverage": "all factions"
}
```

When scrape rules or destination paths are stored in separate local files, change those settings before starting a new collection run.

---

## Requirements

- A web browser for opening the HTML scorecard
- Access to the listings used as the scraper's source
- A local environment that can execute the scraping and export workflow
- Sufficient storage for generated JSON and JS files
- Internet connectivity for collecting current eBay listings

---

## Frequently Asked Questions

**How can I refresh the listings?**  
Run the scraper again and regenerate both the JSON and JS outputs before reopening the viewer.

**Are the results sortable and filterable?**  
Yes. The supplied standalone viewer supports sorting and filtering of the collected listings.

**Are all factions represented?**  
The dataset is designed to cover all factions. The project also identifies a separate Chaos and Be'lakor edition.

**Where does the generated data go?**  
The scraper and export process write the files to the output location configured in your local setup. Inspect that location after generation completes.

**Why is the viewer empty?**  
Verify that scraping finished without errors, then check that the generated JSON or JS files exist and are correctly referenced by the HTML viewer.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
