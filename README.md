# DDEV Addon BOSA a11y

Run BOSA accessibility checker on a URL.

## Installation

ddev add-on get Mschuddings/ddev-bosa_a11y && ddev restart

## Usage

ddev bosa_a11y https://www.politie.be

It will open the report automatically in your browser.

It is possible to test multiple urls via for example:
ddev bosa_a11y https://www.example.be https://www.example2.be https://www.example.be

## Previous reports.

All reports will be in your .ddev/bosa_a11y folder.

## Options

Available standards: "WCAG2A", "WCAG2AA", "WCAG2AAA", "Section508".

They can be passed via for example: "--standard=WCAG2A".
The standard will also be added to the report.

Language is not supported it seems., (or not yet working)
