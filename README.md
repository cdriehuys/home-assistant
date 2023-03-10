# Home Assistant

My Home Assistant config.

## Usage

This configuration does not include everything required for Home Assistant to
function. There are some pieces that should not be hard-coded such as secrets or
information that depends on how Home Assistant is deployed. This configuration
expects to be deployed alongside the following files and directories:

```
/path/to/configuration.yaml
├── themes
│   └── <Any theme files>
├── automations.yaml
├── scenes.yaml
├── scripts.yaml
├── secrets.yaml
└── service-account.json
```

## Secrets

These secrets are expected to be in `secrets.yaml`:

* **`elevation`:** Home elevation in meters. Used for sunrise/sunset times.
* **`google_project_id`:** The ID of the Google project used to connect to
  Google Assistant.
* **`latitude`:** Home latitude for location triggers and weather.
* **`longitude`:** Home longitude for location triggers and weather.
