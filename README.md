# Accelify updates

Version feeds for Accelify's Salesforce packages. Each installed package reads its own product's `latest.json` once a day to tell admins when a newer version is out.

```
<product>/latest.json     the newest promoted version
<product>/versions.json   every promoted version, newest first
```

| Product | Feed |
|---|---|
| Accelify Connect for Xero | `xero/latest.json` |

These files are built from release entries by `tools/release-feed/New-ReleaseFeed.ps1` in Accelify's main repository, through the `/release-feed` skill. Never edit them by hand. They hold only public release information: version numbers, install IDs and release notes.
