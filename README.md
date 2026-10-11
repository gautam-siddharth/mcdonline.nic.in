# Yashvit QR Demo

A Flask demo that displays a clearly labelled test certificate page and generates a QR code pointing to `/certificate.html`.

## Local run

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app.py
```

Open:

http://localhost:3000/

## Generate a QR for a public HTTPS URL

After deploying the application/page publicly, open:

```text
http://localhost:3000/generate-qr?base_url=https://YOUR_PUBLIC_DOMAIN
```

The generated QR points to the public `/certificate.html` URL, so it can be scanned from another device.

## GitHub Pages

GitHub Pages can host static HTML, but it cannot run Flask/Python server code. For GitHub Pages, the certificate page should be converted to a static `index.html`, and the QR should point to the GitHub Pages URL.

This project is intentionally labelled DEMO / TEST and should not be used to impersonate or alter an official certificate.
