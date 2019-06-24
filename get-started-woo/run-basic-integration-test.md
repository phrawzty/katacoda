Now we'll run the integration test on its own:
```
ddev test -m integration awesome
```{{execute}}

This takes a little longer than the unit test since it needs to spin up a Docker environment—but it's still pretty quick. It's possible that you ran into a "linter failure", which looks like this:
```
ERROR:   style: commands failed
```

If you didn't, congratulations! If you _did_, it's very easy to fix—the tooling can even do it for you:


