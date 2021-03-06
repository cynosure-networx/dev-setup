# Homebrew {#homebrew}

Package managers make it so much easier to install and update applications \(for Operating Systems\) or libraries \(for programming languages\). The most popular one for OS X is[Homebrew](http://brew.sh/).

### Install {#install}

An important dependency before Homebrew can work is the**Command Line Tools**for**Xcode**. These include compilers that will allow you to build things from source.

We can install Hombrew! In the terminal paste the following line \(without the`$`\), hit**Enter**, and follow the steps on the screen:

```
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

One thing we need to do is tell the system to use programs installed by Hombrew \(in`/usr/local/bin`\) rather than the OS default if it exists. We do this by adding`/usr/local/bin`to your`$PATH`environment variable:

```
$ echo 'export PATH="/usr/local/bin:$PATH"' 
>
>
 ~/.bash_profile
```

Alternatively, we can also insert`/usr/local/bin`to the first line of`/private/etc/paths`and reboot the Mac to change global paths loading order. Admin password may be required if you modify the file.

Open an new terminal tab with**Cmd+T**\(you should also close the old one\), then run the following command to make sure everything works:

```
$ brew doctor
```

**Install Autojump**

autojump is a faster way to navigate your filesystem. It works by maintaining a database of the directories you use the most from the command line.

_Directories must be visited first before they can be jumped to._

```
$ brew install autojump
```





