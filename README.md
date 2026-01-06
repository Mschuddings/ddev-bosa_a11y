# Deprecated

BOSA checker is deprecated. The BOSA plugin isn't maintained anymore by BOSA so I deprecate this as well.








# Screenshot
![image](https://github.com/user-attachments/assets/fd94af76-6a33-462b-8953-4678f11cee48)


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

It will only open one HTML report but all urls will be checked of course.

## Previous reports.

All reports will be in your ".ddev/bosa_a11y/results" folder.

## Options

Available standards: "WCAG2A", "WCAG2AA", "WCAG2AAA", "Section508".

They can be passed via for example: "--standard=WCAG2A".
The standard will also be added to the report.

Language is not supported it seems. (or not yet working)

Possibility to exclude a certain element ID (for example cookie banner ID)
This can be done via: "--exclude-element-id=XXX"

## FAQ

### How do I test a whole site

Convert your sitemap to CSV via: https://www.bulkgpt.ai/tools/xmltocsv
And then just use that CSV to test your whole website.
