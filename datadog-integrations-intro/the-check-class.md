Alright—let's talk about code. The first thing we'll look at is the check logic itself, which will be expressed as a Python class. If you've worked with Python before, you'll want to know that all Check classes are derived from `AgentCheck`, and that they must provide a `check(self, instance)` method. If you're new to Python—it's cool, don't worry about it!

Checks are organised in regular Python packages under the `datadog_checks` namespace. Practically speaking, this means that your code should live under `awesome/datadog_checks/awesome`. The only hard requirement here is that the name of the package has to be the same as the check name.

Let's take a look at what we've got right now:
```
tree $HOME/dd/integrations-extras/awesome/datadog_checks/awesome/
```{{execute}}

`check.py` looks promising! Let's start there…

### TEST

- `awesome/datadog_checks/awesome/`{{open}}
- `integrations-extras/awesome/datadog_checks/awesome/`{{open}}
- `dd/integrations-extras/awesome/datadog_checks/awesome/`{{open}}
- `$HOME/dd/integrations-extras/awesome/datadog_checks/awesome/`{{open}}
- `/root/dd/integrations-extras/awesome/datadog_checks/awesome/`{{open}}
