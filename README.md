# Bugsnag iOS Crash Report Upload Tool

This tool uploads [iOS crash reports](https://developer.apple.com/library/content/technotes/tn2151/_index.html) to [Bugsnag](https://www.bugsnag.com/) so that they appear as fully symbolicated events in your dashboard.

_NOTE_ - When Bugsnag is configured in an application, crashes are detected and reported automatically. This tool is only required if it is useful to manually upload a crash report.

## Prerequisities
If not already installed, follow [these instructions](https://www.ruby-lang.org/en/documentation/installation/) to install Ruby.

## Usage
```bash
./bin/bugsnag-upload-report <API-KEY> <PATH-TO-CRASH-REPORT>
```

## Finding uploaded reports

To find individual uploaded reports in the Bugsnag dashboard, use the 'Incident Identifier' field which is displayed in the 'Report' tab.

To search for individual reports in the dashboard add a [custom filter](https://docs.bugsnag.com/product/custom-filters/) for the path `metaData.report.Incident Identifier`.
