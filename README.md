# @regrapes/stylelint-config-scss

REGRAPES SCSS-Stylelint config

## Installation

```bash
npm install @regrapes/stylelint-config-scss --save-dev
```

## Usage

Set your stylelint config to:

```json
{
  "extends": "@regrapes/stylelint-config-scss"
}
```

### Extending the config

Add a `"rules"` key to your config, then add your overrides and additions there.

You can turn off rules by setting its value to `null`. For example:

```json
{
  "extends": "@regrapes/stylelint-config-scss",
  "rules": {
    "selector-class-pattern": null
  }
}
```

Or lower the severity of a rule to a warning using the `severity` secondary option. For example:

```json
{
  "extends": "@regrapes/stylelint-config-scss",
  "rules": {
    "property-no-vendor-prefix": [
      true,
      {
        "severity": "warning"
      }
    ]
  }
}
```