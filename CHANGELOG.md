# Changelog

## v1.1.2 — 2026-11-14

- Clearer Marketplace description. User-Agent `quantum-aether-action/1.1.2`. No change to inputs, outputs or behaviour.

## v1.1.1 — 2026-11-14

- An undetermined probe (the scanner could not observe a negotiated key-exchange group, `observation_status: undetermined`)
  is no longer shown as "classical": the job summary says "undetermined" and asks for a re-run.
- With `require-post-quantum: true`, an undetermined result fails the job with an explicit "undetermined" message
  (fail-closed; it already failed before, with a misleading "does not negotiate" message).
- User-Agent `quantum-aether-action/1.1.1`. No change to inputs or outputs.

## v1.1.0 — 2026-11-14

- Default `base-url` is now `https://ather-quantum.com` (was the legacy typo domain `ather-quatum.cloud`).
  The legacy host keeps serving the API, so pinned older versions do not break.
- Guide and "scanned by" links in the job summary point to ather-quantum.com.
- User-Agent `quantum-aether-action/1.1`.
- No change to inputs, outputs or pass/fail behaviour.

## v1.0.1

- Fail closed on unavailable scans (rate limits, server errors, incomplete responses); disclose scan scope.

## v1.0.0

- First release: X25519MLKEM768 check with `require-post-quantum` and `min-grade`.
