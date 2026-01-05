# Sculpt App Universal Deep Links

This repository hosts verification files for universal deep links used in the Sculpt mobile app referral system.

## Files

- `.well-known/apple-app-site-association` - iOS Universal Links verification
- `.well-known/assetlinks.json` - Android App Links verification

> Note: Apple requires the `"apps"` array in `apple-app-site-association` to remain empty for Universal Links; do not add app IDs there because Universal Links now uses the entries under `applinks.details` instead.

## Configuration

- Custom domain: `app.sculptai.io`
- Referral path pattern: `/r/{referralCode}`

## Next Steps

1. Apple Team ID set to `4734C4TSL7` for Universal Links configuration
2. Replace `YOUR_*_SHA256_FINGERPRINT` with your Android app signing certificate SHA-256 fingerprints
3. Configure GitHub Pages to deploy from the main branch
4. Set up custom domain `app.sculptai.io` in GitHub Pages settings
5. Configure DNS CNAME record: `app` -> `your-username.github.io`
