# DDEV Addon BOSA a11y

Run BOSA accessibility checker on a URL.

## Installation

ddev add-on get Mschuddings/ddev-bosa_a11y && ddev restart

## Usage

ddev bosa_a11y https://www.politie.be

It will open the report automatically in your browser.

It is possible to test multiple urls via for example:
ddev bosa_a11y https://www.example.be https://www.example2.be https://www.example.be

### File

It is possible to pass in a *CSV* file.
Please don't use CSV headers.

Then via:
``
ddev bosa_a11y urls.csv
``

The file must be inside of ".ddev/bosa_a11y/config"

It will only open one HTML report though but all urls will be checked of course.

## Previous reports.

All reports will be in your ".ddev/bosa_a11y/results" folder.

## Options

Available standards: "WCAG2A", "WCAG2AA", "WCAG2AAA", "Section508".

They can be passed via for example: "--standard=WCAG2A".
The standard will also be added to the report.

Language is not supported it seems., (or not yet working)

## FAQ

### How do I test a whole site

Convert your sitemap to CSV via: https://www.bulkgpt.ai/tools/xmltocsv
And then jut use that CSV to test your whole website.
