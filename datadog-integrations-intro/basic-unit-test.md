As with the check logic, there's some great sample code for the unit tests in the [Datadog documentation](https://docs.datadoghq.com/developers/integrations/new_check_howto/#writing-tests). Go ahead and paste that code into `dd/integrations-extras/awesome/tests/test_awesome.py`{{open}}.

And, as before, here are some good questions to ask yourself about that code:
- What's being imported? What's purpose might it serve?
- What does the line that starts with `@` mean?
- What elements are being tested, and what happens if they fail?
