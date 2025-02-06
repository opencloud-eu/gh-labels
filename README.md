# GitHub Labels for all Repositories

This repository contains our set of default labels which are to be used in all OpenCloud repositories.

## How to use

The labels are defined in the `.github/settings.yml` file. In order to apply them to a repository, create a 
`.github/settings.yml` file in your repository and add the following content:

```yaml
---
_extends: gh-labels
---
```

If your repository already has a `.github/settings.yml` file, you can just add the `_extends: gh-labels` to the
top of the file.

## Additional labels

If you need additional labels on top of the organization wide labels, you can add them to the `.github/settings.yml` content:

```yaml
---
labels:
  - name: Label-Namespace:Label-Name
    color: "#ffffff"
...
```