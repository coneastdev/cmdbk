# python

Python and pip commands.

Some will be windows only and some linux only, make sure to read which one is which.

## Python terminal

**running python**

```
python
```

This will start the python interpreter, if opened in a console it will take over the console.

If you want to open a file you will need to specify the path, you can use tab to autocomplete the path.

```
py
```

This a shorthand for python, it is used instead of "python" for windows systems.

**If you are on windows, make sure to replace any commands that use "python" with "py"**

---

**quitting python**

```
exit()
```

This is an important command as it lets you exit a python terminal, you can also use the key bind Ctrl+D.

## Virtual environment

**creating a virtual environment**

```
python -m venv venv
```

This will create a virtual environment for you to install dependencies into, the command to activate it is below.

The second "venv" can be changed to whatever you want your virtual environment to be called, usually this is "venv" or ".venv".

If your using git control make sure to add the venv folder, or directory, to your .gitignore. (see git.md for more)

---

**activating the virtual environment**

***WINDOWS ONLY***
```
./venv/Scripts/Activate.ps1
```

This will activate the virtual environment and make any dependencies installed via pip go into the environment only.

Make sure the "./venv/" is the location of your virtual environment if you name it something else or move it from the default position, you  will need to change the "./venv/" to the new path.

***LINUX ONLY***
```
. ./venv/bin/activate
```

This does the same as the windows command but is modified for a bash terminal. The dot at the start is so the program will run in the same terminal you are opening it in.

You may need to edit the executables permissions so it can be run as an executable. You can usually done this via your systems file explorer.

## pip

**Installing packages**
```
python -m pip install
```

```
pip install
```

**uninstalling packages**
```
python -m pip uninstall
```

```
pip uninstall
```

**installing requirements**
```
python -m pip install -r requirements.txt
```

**saving requirements**
```
python -m pip freeze > requirements.txt
```