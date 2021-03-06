Rust Windows Builder Action
========================

![GitHub](https://img.shields.io/github/license/aig787/rust-windows-cross-builder)
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/aig787/rust-windows-cross-builder)
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/aig787/rust-windows-cross-builder/CI)
![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/aig787/rust-windows-cross-builder)

GitHub action for building windows targeted rust binaries (x86_64-pc-windows-gnu). 

```yaml
- uses: aig787/rust-windows-cross-builder@v1.0.4
  with:
    args: build --release --all-features
    credentials: ${{ secrets.GIT_CREDENTIALS }}
```
### Inputs
| Variable | Description | Required | Default |
|----------|-------------|----------|---------|
| args     | Arguments passed to cargo | true | `build --release` | 
| credentials | If provided git will be configured to use these credentials and https | false | |
