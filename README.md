# Yaxii Smart Form - Manifest Files

This repository contains integrity manifest files for Yaxii Smart Form plugin.

## Repository

**GitHub**: https://github.com/ghost4tech/yaxii-manifest

**Raw Content URL**:
```
https://raw.githubusercontent.com/ghost4tech/yaxii-manifest/main/
```

## Manifest Files

- `2.5.1.json` - Version 2.5.1 manifest
- `2.5.2.json` - Version 2.5.2 manifest
- `2.5.3.json` - Version 2.5.3 manifest
- `2.5.4.json` - Version 2.5.4 manifest
- `2.5.5.json` - Version 2.5.5 manifest
- `2.5.6.json` - Version 2.5.6 manifest
- `2.6.0.json` - Version 2.6.0 manifest

## Usage

These manifests are used as fallback endpoints when the primary API is unreachable due to IP reputation blocks or connectivity issues.

## Plugin Configuration

Add to `wp-config.php`:
```php
define('YAXII_MANIFEST_FALLBACK_URL', 'https://raw.githubusercontent.com/ghost4tech/yaxii-manifest/main/');
```

## Security

All manifests are cryptographically signed with ECDSA P-256. The plugin verifies signatures before use.

## Updating

When a new version is released:
1. Generate manifest file
2. Upload to this repository
3. Plugin automatically uses it as fallback

