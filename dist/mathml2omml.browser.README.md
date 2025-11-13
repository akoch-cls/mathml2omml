# mathml2omml.browser.js

This is the bundled browser version of the mathml2omml library.

## What is this file?

This file contains the complete mathml2omml library compiled for browser use. It converts MathML (Mathematical Markup Language) to OMML (Office Math Markup Language) for use in Microsoft Word documents.

## File Details

- **Size**: 2,350 lines (~65KB)
- **Source**: https://github.com/fiduswriter/mathml2omml
- **Format**: UMD (Universal Module Definition) - works in browsers
- **Global variable**: `window.mathml2omml`
- **Main function**: `mathml2omml.mml2omml(mathmlString)`

## How to Use

### In HTML (Direct)

```html
<script src="mathml2omml.browser.js"></script>
<script>
  const mathml = "<math><mi>x</mi></math>";
  const omml = mathml2omml.mml2omml(mathml);
  console.log(omml);
</script>
```

### Via CDN (Recommended for Google Apps Script)

1. **Upload to GitHub Gist or Repository**
2. **Use jsDelivr CDN**:
   ```html
   <script src="https://cdn.jsdelivr.net/gh/YOUR_USERNAME/YOUR_REPO@main/mathml2omml.browser.js"></script>
   ```

## Why CDN for Google Apps Script?

Google Apps Script cannot serve this file directly without corrupting it due to special characters in the JavaScript. Hosting it on an external CDN bypasses this limitation.

## Setup Instructions

See `QUICK_CDN_SETUP.md` for step-by-step instructions on hosting this file on a CDN.
