# Pulse ECG Capture & Report

A small installable mobile web app for photographing an ECG strip or printout and exporting a report.

## Deploy

1. Publish this folder as the root of a GitHub repository.
2. In GitHub, open **Settings → Pages**.
3. Choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. Open the published HTTPS URL on a phone and use **Install app** or the browser's **Add to Home Screen** option.

Camera access requires HTTPS (GitHub Pages provides it). The app requests camera permission only after **Open camera** is tapped. The service worker caches the app shell for offline launch. Image capture and report fields remain in the browser session; reports are generated on device.

Exports: **Save as PDF** uses the browser print dialog; Excel and Word use `.xls` and `.doc` formats compatible with Microsoft Office.

This app captures an image and user-entered details. It does not acquire ECG electrical signals, measure heart activity, interpret ECGs, detect conditions, or provide medical advice.

