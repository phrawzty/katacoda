The `service_check.json` file describes any and all service checks made by the integration. That's it! Grab the sample configuration from the [Datadog integrations documentation](https://docs.datadoghq.com/developers/integrations/new_check_howto/?tab=servicecheck#example-service-check-config) and drop it into `dd/integrations-extras/awesome/assets/service_checks.json`{{open}}.

An important question to consider:
- Is there a relationship between this file and `manifest.json`; specifically, `integration` and `check`?
