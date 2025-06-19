# textlint-rule-preset-unofficial-otel-localization-ja

## About

This is an **unofficial** textlint rule preset for OpenTelemetry Japanese localization.
It was created to improve the efficiency of my Japanese translation activity.
I hope that similar settings will be included in [open-telemetry/opentelemetry.io](https://github.com/open-telemetry/opentelemetry.io) in the future.

## How to Use

This preset uses a simple approach without npm package distribution.
Since this functionality should ideally be integrated into [open-telemetry/opentelemetry.io](https://github.com/open-telemetry/opentelemetry.io), there are no plans to publish it as an npm package.

### 1. Fork and Clone the opentelemetry.io Repository

Fork and clone the [open-telemetry/opentelemetry.io](https://github.com/open-telemetry/opentelemetry.io) repository.
You **do not need to clone** this repository.

### 2. Download the prh Configuration File

In your local opentelemetry.io directory, run the following command to download the prh configuration file:

```bash
wget https://raw.githubusercontent.com/Msksgm/textlint-rule-preset-unofficial-otel-localization-ja/refs/heads/main/otel-localiztion-ja.yml -O otel-localiztion-ja.yml
```

### 3. Update .textlintrc.yml

Add the following configuration to your `.textlintrc.yml` file:

```yaml
rules:
  ## Add the following setting
  prh:
    rulePaths:
      - ./otel-localiztion-ja.yml
  ## End of additional configuration
  terminology: ...
```
