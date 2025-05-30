# Setup QNN SDK

Download and setup Qualcomm AI Engine Direct SDK

## Usage

See [action.yml](action.yml)

<!-- start usage -->
```yaml
- uses: mybigday/setup-qnn-sdk@v1
  with:
    # Which version to download, check version from [official site](https://www.qualcomm.com/developer/software/qualcomm-ai-engine-direct-sdk).
    #
    # Default: 2.32.0.250228
    qnn-sdk-version: ''
```
<!-- end usage -->

**Basic:**

```yaml
steps:
- uses: actions/checkout@v4
- uses: mybigday/setup-qnn-sdk@v1
# your steps
```

The `qnn-sdk-version` input is optional.

The action will first check the cache for a semver match. If unable to find a specific version in the cache, the action will attempt to download a version of SDK.

## License

The scripts and documentation in this project are released under the [MIT License](LICENSE)
