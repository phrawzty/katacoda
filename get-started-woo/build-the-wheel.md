Next stop: the wheel. Wheels are a Python-native packaging format. If you've ever used RPM or DEB files, for example, you've encountered a packaging format—wheels are quite similar. And, like all packaging formats, you can tumble down the rabbit hole fairly easily. Luckily for us, the `ddev` tooling takes care of the heavy lifting:
```
ddev release build awesome
```{{execute}}

The output contains an important line: the path and filename of the wheel file that was built. Make a note because we're going to use that to install and activate the integration.
