## What is Python

- Python is a high-level, interpreted programming language known for its simplicity and readability.
- It was created by Guido van Rossum and first released in 1991.
- Python emphasizes code readability and a syntax that allows programmers to express concepts in fewer lines of code than would be possible in languages like C++ or Java.
- It supports multiple programming paradigms, including procedural, object-oriented, and functional programming styles.
- Python has a large and active community of developers who contribute to its extensive standard library and numerous third-party packages, making it suitable for a wide range of applications, including web development, data analysis, artificial intelligence, scientific computing, game development, and more.
- Python's popularity has been steadily increasing due to its versatility, ease of learning, and wide range of applications. It's widely used in both academia and industry, and its popularity continues to grow.

## Install Python

To install Python on your system, follow these steps:

1. **Download Python**: Go to the official Python website at https://www.python.org/ and navigate to the Downloads section. Choose the version of Python you want to install (usually the latest stable version, which should be prominently displayed), and select the appropriate installer for your operating system.
2. **Run the Installer**: Once the installer is downloaded, run it by double-clicking on the downloaded file. This will launch the Python installer.
3. **Configure Installation Settings**: Follow the prompts in the installer to configure Python installation settings. You may need to choose installation options such as the installation directory, adding Python to your system's PATH, and customizing installation features. For most users, the default settings are sufficient.
4. **Install Python**: Proceed with the installation by clicking on the "Install" or "Next" button, depending on the prompts provided by the installer. The installation process may take a few minutes to complete.
5. **Verify Installation**: After the installation is finished, you can verify that Python has been installed correctly by opening a command prompt (on Windows) or terminal (on macOS or Linux) and typing `python --version` or `python3 --version`. This command should display the installed Python version.

Once Python is installed, you can start using it to run Python scripts, execute Python commands interactively, or develop Python applications.

Note: If you're using a Linux distribution, Python is often pre-installed. However, you can use package managers like `apt` (for Debian/Ubuntu-based systems) or `yum` (for Red Hat/CentOS-based systems) to install Python if it's not already available. For example, on Ubuntu, you can use the following command to install Python 3:

```
sudo apt update
sudo apt install python3

```

Similarly, on CentOS, you can use `yum`:

```
sudo yum install python3

```

Replace `python3` with `python` if you want to install Python 2 (though Python 2 is officially deprecated and not recommended for new projects).

## Python interpreter

To access the Python interpreter, follow these steps:

1. **Open a Command Prompt or Terminal**: Depending on your operating system, open a command prompt (on Windows) or terminal (on macOS or Linux).
2. **Type `python` or `python3`**: Once the command prompt or terminal is open, type `python` if you're using Python 2, or `python3` if you're using Python 3, then press Enter. This will launch the Python interpreter.
3. **Start Using the Python Interpreter**: After launching the Python interpreter, you'll see a prompt (typically `>>>`) where you can start typing Python commands. For example, you can try typing `print("Hello, world!")` and press Enter. You should see the output `Hello, world!` printed on the next line.
4. **Exit the Interpreter**: To exit the Python interpreter, you can type `exit()` or press `Ctrl + D` (on Unix-like systems) or `Ctrl + Z` followed by Enter (on Windows).

Here's an example of what you would see in the terminal:

```python
$ python3
Python 3.8.10 (default, May  3 2021, 08:31:45)
[Clang 12.0.5 (clang-1205.0.22.9)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hello, world!")
Hello, world!
>>> exit()
$

```

That's how you access and use the Python interpreter on your system.

## Code editors

There are numerous code editors available, each with its own set of features and advantages. Here are some popular ones:

1. **Visual Studio Code (VS Code)**: Developed by Microsoft, Visual Studio Code is a highly customizable code editor with built-in support for a wide range of languages, including Python. It offers features like IntelliSense, debugging support, Git integration, and an extensive ecosystem of extensions.
2. **PyCharm**: PyCharm is a full-featured Python IDE developed by JetBrains. It offers advanced features tailored specifically for Python development, such as code analysis, refactoring tools, integrated version control, and support for web development frameworks like Django and Flask.
3. **Sublime Text**: Sublime Text is a lightweight yet powerful text editor known for its speed and simplicity. It offers features like multiple selections, a command palette, and a wide range of plugins and packages that enhance its functionality, including Python support.
4. **Atom**: Atom is an open-source text editor developed by GitHub. It's highly customizable through packages and themes and provides built-in Git integration, smart autocompletion, and other features suitable for Python development.
5. **Spyder**: Spyder is an open-source IDE designed specifically for scientific computing and data analysis with Python. It provides a MATLAB-like interface with features such as an integrated IPython console, variable explorer, and support for plotting libraries like Matplotlib.
6. **Jupyter Notebook**: Jupyter Notebook is an open-source web application that allows you to create and share documents containing live code, equations, visualizations, and narrative text. It's widely used for data analysis, machine learning, and interactive Python development.
7. **IDLE**: IDLE (Integrated Development and Learning Environment) comes bundled with Python and provides a simple integrated development environment for Python. While it lacks some advanced features found in other editors, it's suitable for beginners and lightweight scripting tasks.

These are just a few examples, and there are many other code editors and IDEs available. The choice of code editor ultimately depends on your personal preference, workflow, and specific requirements for your Python projects.

## Your first Code

Certainly! Here's a simple "Hello, World!" program in Python:

```python
print("Hello, World!")

```

Now, let's break down this code and explain each part:

1. `print`: `print` is a built-in Python function used to output data to the console. It takes one or more arguments and displays them as text.
2. `"Hello, World!"`: This is a string literal enclosed in double quotes. It's the text that we want to display on the console. In this case, it's the classic "Hello, World!" message, which is commonly used as a first program when learning a new programming language.

When you run this Python program, the `print()` function is called with the argument `"Hello, World!"`, and it displays that text on the console.

To run this code:

1. Open a text editor (such as Notepad, Sublime Text, Visual Studio Code, etc.) on your computer.
2. Copy and paste the above code into the text editor.
3. Save the file with a `.py` extension, for example, `hello.py`.
4. Open a command prompt or terminal.
5. Navigate to the directory where you saved the `hello.py` file.
6. Type `python hello.py` (or `python3 hello.py` if you're using Python 3) and press Enter.

You should see the output `Hello, World!` printed on the next line in the console.

Congratulations! You've just written and executed your first Python program. The "Hello, World!" program is a simple introduction to Python syntax and how to use the `print()` function to output text. It's often the first step in learning a new programming language.

## VS Code Shortcuts

### **Delete the current line: Ctrl + Shift+ K**

Imagine you were to delete your lines by finding your line with the mouse cursor, selecting your line with a double click and then pressing delete — now compare this to using Ctrl + Shift + K — you’re most likely already at the line with your keyboard cursor, so there’s virtually no overhead to deleting it. I use it all the time.

### **Select current line: Ctrl + L**

Selecting the line is also a pretty involved process, as you need to find the line you’re already at with your mouse cursor and then double-click it, which can usually throw you off your keyboard-based flow greatly. This one is a serious timesaver.

### **Select current word: Ctrl + D**

Lately I've also been using Mac OS a lot and have found it incredibly challenging to select the current word with my touchpad. Ctrl + D (or, well, the Mac alternative to it) comes to the rescue.

### **Move line: Alt + Up/Down**

Moving lines around is something I do practically all day. Imagine you were to find the line with your mouse cursor, selecting it with a double click, copying it with a right click and selecting Copy, deleting it with Delete, finding the line you want to insert it at with your mouse cursor, creating a new line, then pasting it with a right click and selecting Paste. Try using the simple alternative — Alt + Up/Down. It will save you a ton of time and I guarantee you that it will provide you with a smoother and more enjoyable development experience.

### **Indent/outdent line: Ctrl + ([/])**

While you could use the standard Tab and Shift + Tab, this would require you to be at the start of the line to outdent, which is not ideal. Ctrl + [ or Ctrl + ] to the rescue!

### **Select all occurrences of a variable: Ctrl + D && Alt + Enter**

This is particularly useful for variable renaming. You select the current word with Ctrl +D or just move your cursor to it and press Alt + Enter and voilà! You will be able to rename it seamlessly, saving you a ton of time.

### **Automatic import: Ctrl + I**

This will give you a list of suggestions for importing a class, interface, etc. that you are trying to use and then auto import it upon selection. I cannot begin to explain how useful this is. It does not always work perfectly, especially if it’s the first time importing something into a project, but in most other cases it will work perfectly. It will save you a ton of time compared to either finding the right import statement or copying it from somewhere else.

### **Search files by name: Ctrl + P**

Using the file explorer on the left is fine, but when you’re really familiar with the project, you usually know exactly what you’re looking for — filename wise. As a result, using Ctrl + P and typing the first couple of characters to open a file will be much faster.

### **Finding references to a function: Alt + Shift + F12**

Finding references to a function is something I do all the time, especially during code reviews and such. I, however, do find this shortcut a bit hard to remember and my keyboard has the sleep button on F12 by default, so there’s no room for mistakes.

### **Move up and down in the file: Ctrl + Up/Down**

Instead of resorting to the cursor while in keyboard mode to scroll up or down the currently open file, just use Ctrl + Up or Ctrl + Down. You could use PgUp or PgDown too, but these are usually farther away from the keys you use all the time.

### **Open find in workspace: Ctrl + Shift + F**

I find myself searching for things workspace-wide all the time and it’s really tedious to break out of a keyboard-based workflow just to open the find in workspace panel.

### **Open the terminal pane: Ctrl + `**

I’m constantly using the built-in terminal in VSCode. This will bring it forward regardless of where you are.

### **Open a new terminal in the terminal pane: Ctrl + Shift + 5**

You will most often need more than one instance of the built-in terminal. Instead of always searching for the icon to split the pane, use this great keyboard shortcut.

### **Open a folder in a new instance: Ctrl + Shift + N && Ctrl + K && Ctrl + O**

I often surf between different projects in VSCode and find myself wanting to open a new one all the time. For this, you open a new VSCode window with Ctrl + Shift + N, then open the folder selector with Ctrl + K && Ctrl + O. Voila!

And, of course, there are some that are useful outside of VSCode:

### **Close tab: Ctrl + W**

This is a standard shortcut to close tabs, and if you do not use it, you really should.

### **Change text size: Ctrl + (+/-)**

Especially useful when showcasing your work in a Zoom meeting, the default text is usually too small to see on a compressed video stream.

### **Find in file: Ctrl + F**

Probably not much is needed to say about that, because you should already be using it everywhere.

## Python Extensions

[Top 10 VS Code Extensions For Python[2024] - GeeksforGeeks](https://www.geeksforgeeks.org/top-10-vs-code-extensions-for-python/)
