Next up is the `manifest.json` file, generally referred to simply as "the manifest". This file describes the opereating parameters of the integration, and is used by Datadog to help position the integration within the greater eco-system. Accordinly, the contents of this file are not generally used by the integration itself, which means it's not necessary for the integration to function; however, without a correctly populated manifest, a given integration cannot be included upstream.

The [Datadog integrations documentation](https://docs.datadoghq.com/developers/integrations/new_check_howto/#manifest-file) covers the contents of this file extensively. Let's take a look at the `awesome/manifest.json`, which was created by the scaffolding. In particular, note:
- `guid`: _Must_ be unique; you [probably](https://en.wikipedia.org/wiki/Universally_unique_identifier#Collisions) don't need to touch this. 😉
- `short_description`: A short description of the integration.
- `categories`: This corresponds to the [list of integration categories](https://docs.datadoghq.com/integrations/); in this case, let's classify it as `web`.
- `is_public`: 

Finally, note the reference to the `service_checks` asset, because that's where we're headed next!
