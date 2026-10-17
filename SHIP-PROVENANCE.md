# Native npm upstream acceptance

Upstream: https://github.com/timlrx/tailwind-nextjs-starter-blog
Commit: b45bef66b40c63b6f57c15ee8cd090682238df4c
MIT license preserved. All content and application components retained.

Adaptations: generated package-lock.json for npm reproducibility; production start script; external newsletter, comments and analytics disabled in public test configuration. No provider credentials. Package versions and dependency graph remain upstream.

Local upstream defect: React hydration mismatch in the closed Headless UI MobileNav portal (server span vs client div). Preserved raw failed Chromium run. Adaptation mounts that portal after hydration, retaining mobile navigation. Production browser is rerun after the fix.

The upstream commit hook required an unavailable yarn executable. Package manager metadata now names the npm version used for acceptance; lint-staged invokes the installed eslint/prettier binaries directly. Hooks remain enabled. Original yarn.lock retained unchanged for provenance.
