Alright—let's get into some code. The first thing we'll look at is the check logic itself, which will be expressed as a Python class. If you've worked with Python before, you'll want to know that all Check classes are derived from `AgentCheck`, and that they must provide a `check(self, instance)` method. If you're new to Python, don't worry about it!

Checks are organized in regular Python packages under the `datadog_checks` namespace. Practically speaking, this means that your code should live under `awesome/datadog_checks/awesome`. The only hard requirement here is that the name of the package has to be the same as the check name.

Let's create a Service Check named `awesome.search` that searches for a string on a web page. It will result in `OK` if the string is present, `WARNING` if the page is accessible but the string was not found, and `CRITICAL` if the page is inaccessible. The code will live in `awesome/datadog_checks/awesome/awesome.py`.
