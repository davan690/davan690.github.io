# Security Audit Report and Task List

## Summary

I reviewed the repository for common security issues across configuration, templates, static files, and site content. The active production site is now materially hardened: there are no obvious hardcoded AWS keys, GitHub tokens, or private-key materials in the tracked source files reviewed, and the current Jekyll build configuration no longer exposes the previously high-risk settings.

The remaining risk is limited to archival and draft content that is not part of the active published build. This content should still be reviewed or cleaned up opportunistically, but it is not presently a live security exposure for the main site.

## Key Findings

### 1) No obvious exposed secrets found
- No clear AWS access keys, GitHub PATs, private keys, or credential material were found in the reviewed repository content.
- Public IDs and social metadata are present in configuration, but they are not secrets in the same class as API keys or tokens.
- This has been checked in [_config.yml](_config.yml), [staticman.yml](staticman.yml), and the site include templates.

### 2) Production hardening was applied
- A Content Security Policy was added in [_includes/head.html](_includes/head.html).
- Staticman was hardened in [staticman.yml](staticman.yml) by enabling moderation and restricting allowed origins.
- The GitHub Actions workflow in [.github/workflows/codeql-analysis.yml](.github/workflows/codeql-analysis.yml) was updated to current supported CodeQL action versions.
- [SECURITY.md](SECURITY.md) was replaced with a real disclosure policy instead of a placeholder template.

### 3) Legacy mixed-content URLs remain mainly in non-published draft content
- The repository still contains some plain `http://` links in historical drafts and legacy notes.
- These are not in the active site build and do not materially impact the live production site, but they can still create mixed-content warnings if those files are published or used as examples.
- This is an archival-content cleanup task rather than an active site compromise.

### 4) Raw script and iframe patterns are still present in old drafts
- Some older draft files contain embedded scripts or inline iframe markup.
- These are historical examples rather than active production content, but they should still be sanitized or archived away from the live site before reusing or publishing them.

## Current Status

### Resolved
- [x] Remove or sanitize the previously identified raw script/iframe risks in the active repository configuration and build content.
- [x] Review and fix the main mixed-content issue in the active site content.
- [x] Harden Staticman comment handling.
- [x] Upgrade the CodeQL workflow to current versions.
- [x] Replace the template placeholder security policy with a real vulnerability-reporting process.

### Remaining / Deferred
- [ ] Clean up legacy plain `http://` links in non-published draft content and historical notes.
- [ ] Remove or isolate old embedded script/iframe examples from draft files that are not intended for production use.
- [ ] Optionally perform a stricter git-history scan across all branches and tags if a full repository-history credential audit is required.

### Low Priority / Monitoring
- [ ] Keep external tracking and analytics integrations reviewed for necessity and privacy impact.
- [ ] Continue to review new embedded scripts, widgets, and third-party content before publishing.

## Recommended Next Step

The production repository is in a much better security state and there are no remaining active-site issues that match the original high-risk findings. If a stricter “full history” audit is desired, the next targeted step is a branch-and-tag credential sweep; otherwise the current repo is suitable for continued maintenance without immediate critical remediation.
