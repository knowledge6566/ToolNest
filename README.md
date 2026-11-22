# ToolNest — All-in-One Online Tools

A static website made with HTML, CSS and JavaScript. No Node.js, database, login or backend is required.

## Included tools
- Image compressor (JPG/PNG/WebP input)
- Image resizer (custom width and height, optional aspect ratio)
- Merge PDF files
- Extract selected PDF pages (for example `1, 3-5`)
- Rotate PDF pages
- Convert images to PDF
- QR code generator with PNG download
- Word and character counter
- Text case converter
- Remove extra spaces
- Age calculator
- Percentage calculator
- Length converter

## Libraries and internet
PDF actions use PDF-Lib and QR generation uses QRCode.js from cdnjs CDN. Those features need internet access when the page loads. Selected files are processed locally in your browser and are not uploaded to this website's server.

## Preview
Because browsers may block loading `tools.json` from a `file://` URL, preview this static site from its folder using:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`. This is only a local static-file preview, not a backend.

## Publish free with GitHub Pages
1. Create a GitHub repository and upload `index.html`, `style.css`, `script.js` and `README.md`.
2. Go to **Settings → Pages**.
3. Select **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
4. For `tools.nishublogs.online`, add that custom domain in Pages settings.
5. In your DNS manager add a CNAME: Host `tools`, Target `<your-github-username>.github.io`.
6. Wait for DNS and HTTPS provisioning.

## Customize
Edit `index.html` for page content, `style.css` for design, and `script.js` for tools and functionality. Third-party CDN libraries should be kept or replaced with equivalent local files if you need offline operation.
