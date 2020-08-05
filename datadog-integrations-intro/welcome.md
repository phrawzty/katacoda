Welcome to the Intro to Datadog Integrations course! The interface you see in your browser right now is what we'll use to install and configure software, write code, and have some fun learning about Linux, Python, and Datadog. There are three panels:
1. This panel, which is where text content, instructions, and challenges are presented.
1. The panel in the upper-right, which is a combination file explorer and text editor.
1. The panel in the lower-right, which is a terminal on a real live Linux system.

The file explorer can be used to navigate the file system, create files and folders, and open files for editing. Let's try:
* Right-click on `/root`, then navigate through New ▶ File.
* Name the file `Hello_world`.
* Click on `Hello_world` to open the file in the editor (feel free to type something).
* Close the file by clicking on the little `x` in the tab above the editor panel.
  * Note the _lack_ of a save button…
* Delete the file by right-clicking on it in the explorer and navigating to Delete.

When this course was loaded, a small series of initialisation actions (generally referred to as "init") kicked off. The init will be complete when you see `You're good to go!`. Oh, one last thing: whenever you see some `fixed-width text` with a ⏎ following it, that means you can click on the text to execute that command in the terminal. For example: `echo "Hello, World!"`{{execute}}

Your first challenges:
- Run a command directly in the terminal (try `echo "hi"`).
- Move on to the next step.

## TEST

### paths

* `mkdir $HOME/one/`{{execute}}
* `touch $HOME/one/1.txt`{{execute}}
* `mkdir two/`{{execute}}
* `touch two/2.txt`{{execute}}
* `mkdir /root/three/`{{execute}}
* `touch /root/three/3.txt`{{execute}}

### pushd

* `mkdir -p $HOME/dd/integrations-extras/awesome/datadog_checks/awesome/`{{execute}}
* `pushd $HOME/dd/integrations-extras/`{{execute}}
* `pwd`{{execute}}

### touch

* `touch $HOME/dd/integrations-extras/awesome/datadog_checks/awesome/1.txt`{{execute}}
* `touch awesome/datadog_checks/awesome/2.txt`{{execute}}

### opens from $HOME

* `popd`{{execute}}
* `pwd`{{execute}}
* `$HOME/dd/integrations-extras/awesome/datadog_checks/awesome/1.txt`{{open}}
* `/root/dd/integrations-extras/awesome/datadog_checks/awesome/1.txt`{{open}}
* `dd/integrations-extras/awesome/datadog_checks/awesome/1.txt`{{open}}

### opens from pushd?

* `pushd $HOME/dd/integrations-extras/`{{execute}}
* `pwd`{{execute}}
* `awesome/datadog_checks/awesome/2.txt`{{open}}

### env var

* `export DD=$HOME/dd/integrations-extras`{{execute}}
* `popd`{{execute}}
* `ls $DD/awesome`{{execute}}
