
# Knowledge Pack Format

User-initiated import only.

## Structure

pack/
  manifest.json
  content/
  index/
  signature.sig

## Security

- Ed25519 signature verification
- Hash validation
- Explicit user trust store

## Distribution

- GitHub Releases recommended
- LAN share or manual import allowed
