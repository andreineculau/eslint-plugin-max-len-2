# max-len-2 (eslint plugin)

Ref: https://github.com/eslint/eslint/issues/6910

Usually I have a soft-limit of 80 characters per line,
and a hard-limit of 120 characters per line.

Since eslint rules cannot set the error level (warn/error) themselves,
this copy of the built-in "max-len" rule (that comes with **your own eslint installation**),
allows you to define soft and hard limits in your `.eslintrc.yaml` like this:

```yaml
  max-len:
    - error
    - code: 120
      ignoreComments: true
      ignoreUrls: true
  max-len-2/max-len-2:
    - warn
    - code: 80
      ignoreComments: true
      ignoreUrls: true
```

## License

MIT
