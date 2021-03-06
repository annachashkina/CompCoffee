# Getting ready: Windows
Here you can find some tips on how to prepare your machine and install minimum required software.

## *Git*
*Git* is a powerful version control tool. It allows collaborators to contribute to the same project and helps keep track of all changes made to the code. *Git*-based tools are usually console-oriented and can be used from terminal. Under **Windows** *Git* is available [here](https://git-scm.com/download/win). During installation process, make sure you check following options
- Use git from the Windows Command Prompt
- Use the OpenSSL library
- Checkout as-is, commit as-is
- Use Windows' default console window
- Enable file system caching
- Enable Git Credential Manager

To check that everything is OK, open your preferred terminal and type
```
git status
```
You should get an output message similar to this 
```
fatal: Not a git repository (or any of the parent directories): .git
```
This simply means that directory you are in is not a *git repository. It also means *Git* is installed and working fine.

During this course, we use *GitHub*, a web-based *Git*, as a storage place for tutorial code and manuals (like the one you are reading). 
For **Windows** *GitHub* provides easy-to-use application (available [here](https://desktop.github.com/)). You can also manage *GitHub* repositories through terminal, using *Git*, installed during previous step.

## *Python*
1. In order to install *Python*, you need to first download intallation file from [python.org](https://www.python.org/downloads/). You can install both 3.* and 2.* versions.
**[Note]** From now on, instructions are provided for *Python 3.*, but simillar comands should work fine with older versions.
2. Make sure you have selected the latest version. During installation, check that **pip** is installed. 
3. **[Optional]** A good idea is to add path to *Python* executable to system's **PATH** variable. It can also be done during installation phase. In that case you can access *Python* interactive shell from your *CMD* or *PowerShell*.
4. Now check that everything is OK. Open your preffered shell (*CMD* or *PowerShell*).
    
    4.1. If you decided to add *Python* directory to system's **PATH**, then type
    ```
    python --version
    ```
    and continue to step **5**.
    
    4.2. If you skipped step **3**, navigate to *Python* installation dir and type
    ```
    .\python.exe --version
    ```
    and continue to step **5**.
5. If everything is OK, you will get an output, similar to this: 
```
Python 3.6.2
```
6. **[Optional]** With *Python* set up preoprly, you can check and install several packages. 
The must-have packages for a scientist are *matplotlib* and *numpy*. Another good one is *ipython*. To install a package, perform procedure, similar to the one discussed in **4**. Run following command (to e.g. install *matplotlib*):
```
python -m pip install matplotlib
```
If the output says that you already have this package, consider upgrading it but invoking similar command
```
python -m pip install matplotlib --upgrade
```
Do the same for remaining packages.

## Development tools: Text/Code editors vs. IDEs
It is possible to edit code using lots of different tools: starting from console and up to powerful IDEs (**I**ntegrated **D**evelopment **E**nvironment). You can use whatever tool you like, however, here are a few suggestions.
1. **Text Editor.** If you want to use just plain text editor, consider using [*Visual Studio Code*](https://code.visualstudio.com/). It is a powerful extendable crossplatform editor. It has a range of useful *Python*-oriented plugins that can be used in the process of development. Great advantages of this tool are **IntelliSense** (helps you type function names and access class methods/fields) and **Debuggers** (allow you to execute your program step by step, inspecting any variable at any time. Greatly helps when you struggle to find a bug).
To install it, download apropriate version and follow the instructions. After installation has finished, open a new window of *Visual Studio Code*, navigate to **Extensions** (or hit `Ctrl + Shift + X`, by default) and search fot *Python*. Then you can download extentions that will help you code better in *Python*.
**[Note]** This guide is written in *Visual Studio Code*.

2. **IDE.** On a **Windows** machine there is probably no better **IDE** than [*Visual Studio*](https://www.visualstudio.com/downloads/). Its *Community* version is free for students, researchers, non-profit developers, etc., so you can freely use it for your own purposes. *VS* contains numerous tools, including *Python* tools (called **P**ython **T**ools for **V**isual **S**tudio). It is also great for developing using *C*/*C++* for any platform. 
*VS* also supports various plugins, provides **IntelliSense** and **Debugger** for *Python* projects. Essentially, it is **the** ultimate tool, but its size can reach 10-20 GBs and you need to first play with it a little bit to get used to and learn how to work with it.
To install it, follow the installation instructions after downloading apropriate installer.

3. **Any other tool**. Essentially, you can use anything, but the power of **advanced** editors is in their tools that help you develop faster, better, make less mistakes and keep your code clean.
