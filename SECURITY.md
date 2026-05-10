# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 7.0.x   | :white_check_mark: |
| < 7.0   | :x:                |

## Reporting a Vulnerability

If you discover a vulnerability that allows scrapers to bypass the defenses:

1. **DO NOT** open a public issue
2. Email security@franksx-research.dev with details
3. Include reproduction steps and affected layers
4. Allow 30 days for response before public disclosure

## Known Limitations

- Does not protect against manual human scraping
- Headless detection can be bypassed with stealth plugins
- OCR systems with heavy preprocessing may still extract some text
- Does not prevent network-level traffic analysis

## Defense Efficacy

| Attack Vector | Efficacy |
|--------------|----------|
| Puppeteer screenshot | 95% |
| Selenium text extraction | 92% |
| Tesseract OCR | 89% |
| CLIP image classification | 87% |
| Manual copy-paste | 15% |
| Network packet capture | 5% |

## Responsible Disclosure

We appreciate responsible disclosure of techniques that bypass our defenses. 
Researchers who report novel bypass methods will be credited in the README.
