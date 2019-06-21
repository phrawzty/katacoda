Finally—it's time to write some code! We'll create a Service Check named `awesome.search` that searches for a string on a web page. It will result in `OK` if the string is present, `WARNING` if the page is accessible but the string was not found, and `CRITICAL` if the page is inaccessible.

There's some great sample code available in the [Datadog documentation](https://docs.datadoghq.com/developers/integrations/new_check_howto/#implement-check-logic) that you can just copy and paste into `awesome/datadog_checks/awesome/awesome.py` directly. There are two ways to edit files in this tutorial environment:
- Using an editor such as `vim` or `nano` directly in the shell
- Via the built-in editor in the upper right of this window
