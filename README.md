# golint

> Golint is a linter for Go source code. https://github.com/golang/lint

[![wercker status](https://app.wercker.com/status/e3512f90373e7eb59131c2c70c5da7a5/m/master "wercker status")](https://app.wercker.com/project/bykey/e3512f90373e7eb59131c2c70c5da7a5)

# Options

- `exclude` (optional) Exclude certain files. Uses `grep -ve` to do the exclude.

# Examples

```yaml
build:
    steps:
        - golint
```

Using an exclude filter:

```yaml
build:
    steps:
        - golint:
            exclude: "\.pb\.go"
```

# License

The MIT License (MIT)

# Changelog

## 1.2.0

- Add support for excluding files.

## 1.1.0

- Do not report on zero issues.

## 1.0.0

- Initial release.
