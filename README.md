# Refy Journal

<p align="center">
  <img src="icono.png" alt="Refy Journal icon" width="96">
</p>

Refy Journal is a local-first journaling web app for writing daily entries, rating each day, tagging activities and emotions, and reviewing personal trends over time.

## Features

- Create one journal entry per date.
- Add a title, free-form text, and a numeric day rating.
- Tag entries with customizable activities and emotions.
- Edit the available activity and emotion tags from the app.
- View saved entries with filters for all time, year, month, or a specific month.
- Analyze mood trends, activity frequency, and emotion distribution.
- Filter analytics by month, previous month, six months, year, all time, a specific month, or a custom date range.
- Export entries to JSON or CSV.
- Import JSON backups.
- Stores data locally in the browser with `localStorage`.

## Dynamic Tags

Activities and emotions are editable. The editor shows the currently active tags, while analytics uses the tags that actually appear in entries for the selected date range. This means older or removed tags can still appear in historical analytics if past entries used them.

JSON exports preserve both entries and the current tag lists. CSV exports include active tags as well as historical tags found in the exported entries.

## Tech Stack

- HTML
- CSS
- JavaScript
- [Chart.js](https://www.chartjs.org/) for analytics charts
- [Hammer.js](https://hammerjs.github.io/) and `chartjs-plugin-zoom` for mobile chart interactions


## Project Context

This project was built as a personal journaling tool focused on quick daily reflection and lightweight self-analysis. It combines written entries with structured mood, activity, and emotion tracking so patterns can be reviewed over time.

## Limitations

- Data is stored only in the current browser unless exported manually.
- There is no account sync or cloud backup.
- Importing a JSON backup replaces the current journal data.
- Analytics depend on external CDN libraries.

