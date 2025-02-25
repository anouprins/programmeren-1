# Windows 8: Installing

To develop with a C compiler you will need some tools on your laptop. This guide helps you to install these tools and a code editor.

Note: These instructions are written for Windows 8. If you are using Windows 10 or newer please follow [these](/extra/installatie/windows) instructions.

## Step 1: Git

Head to [the git website](https://git-scm.com/downloads) and download git for windows.

During the installation change the following options

![Choose "Use the Nano editor by default"](git_nano.png)

![Choose "Use Windows' default console window](git_terminal.png)

## Step 2: Sass

Download sass from [GitHub](https://github.com/sass/dart-sass/releases/), `dart-sass-x.xx.x-windows-ia32.zip` for 32-bits Windows and `dart-sass-x.xx.x-windows-x64.zip` for 64-bits Windows.

[Is my windows 32 or 64 bits?](https://www.howtogeek.com/howto/21726/how-do-i-know-if-im-running-32-bit-or-64-bit-windows-answers/)

Extract the zip you've downloaded

Click "Extract All"

![](sass_extract1.png)

And extract it to `C:\`

![](sass_extract2.png)

If you want to use Sass from the terminal you'll need to add it to you 'PATH'.

1. The first step depends which version of Windows you're using:
    - If you're using Windows 8 or 10, press the Windows key, then search for and
    select "System (Control Panel)".
    - If you're using Windows 7, right click the "Computer" icon on the desktop
    and click "Properties".
2. Click "Advanced system settings".
3. Click "Environment Variables".

![](sass-path1.png)

4. Under "System Variables", find the `PATH` variable, select it, and click "Edit".

![](sass-path2.png)

5. Click "New" and "Browse..."

![](sass-path3.png)

6. Navigate to your `C:\` drive and click "dart-sass"

![](sass-path4.png)

7. Click (all the) "Ok"-buttons(s) to save the settings

Open "Git Bash" from the Start menu.

Run

    echo 'alias sass=/c/dart-sass/sass.bat' >> ~/.bash_profile; source ~/.bash_profile

to make it easier to run `sass`
Now you should be able to use sass, execute `sass --version` in your terminal to verify this.

## Step 3: Python3

Download Python 3.9 from the [Python website](https://www.python.org/downloads/).

Install Python, make sure you check the "Add Python 3.9 to PATH" box.
![](python.png)

## Step 4: Atom


Download and install [Atom](https://atom.io/).



## Troubleshooting
Ran into trouble? Contact the staff! It’s important to get started quickly. You only have to do the above once, so get help now and you’ll be set for the remainder of the course!
