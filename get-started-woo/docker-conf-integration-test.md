There are lots of ways to accomplish our goal. One popular technique is to use Docker to spin up a very small, very lightweight environment that meets the needs of the testing scenario. In our case, we'll use it to set up and run a web server, query that server for a page, and then analyse the result acording to our check logic.

We'll start by setting up a Docker configuration. Head back to the [testing section](https://docs.datadoghq.com/developers/integrations/new_check_howto/#writing-tests) of the Datadog integration documentation and look for `awesome/tests/docker-compose.yml`. Copy and paste for the win!

As always, it's good to ask some questions:
- Which web server software will be installed?
- What port will be exposed to our test harness?
