With Docker out of the way, we can concentrate on the test itself. There are two separate but related components to consider: the _configuration_ of the test, and the _instantiation_ of that configuration (i.e. actually running the test).

We'll start with the configuration. Thinking back to the test-related files that the harness prepared (`tree $HOME/dd/integrations-extras/awesome/tests/`{{execute}} if you need a reminder), note the `awesome/tests/conftest.py` file. That's a great spot to put _conf_iguration for _test_s. 😀

