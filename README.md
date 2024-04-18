# unsupported-range-renovate-python

### Expected

Renovate handles version syntax like `^0.43b0`

### Actual

Renovates doesn't seem to support that particular range syntax

## Support

Opened the ticket at https://github.com/renovatebot/renovate/discussions/28480

## Renovate Log

<details>
  <summary>Click to expand</summary>

  ```shell
DEBUG: packageFiles with updates
{
  "baseBranch": "main"
  "config": {
    ...
    "poetry": [
      {
        "deps": [
          ...
          {
            "datasource": "pypi",
            "currentValue": "^0.43b0",
            "managerData": {
              "nestedVersion": false
            },
            "skipReason": "invalid-version",
            "depName": "opentelemetry-instrumentation-requests",
            "depType": "dependencies",
            "lockedVersion": "0.43b0",
            "updates": [],
            "packageName": "opentelemetry-instrumentation-requests"
          },
          ...
        ]
      }
    ]
  }
}
  ```
</details>
