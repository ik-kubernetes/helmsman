---
version: v1.8.0
---

# Protecting apps (releases)

You can define apps to be protected using the `protected` field. Please check [this doc](../protect_namespaces_and_releases.md) for details about what protection means and the difference between namespace-level and release-level protection.

Here is an example of a protected app:

```toml
[apps]

    [apps.jenkins]
    namespace = "staging"
    enabled = true
    chart = "stable/jenkins"
    version = "0.9.1"
    protected = true # defining this release to be protected.
```

```yaml
apps:

  jenkins:
    namespace: "staging"
    enabled: true
    chart: "stable/jenkins"
    version: "0.9.1"
    protected: true # defining this release to be protected.
```
