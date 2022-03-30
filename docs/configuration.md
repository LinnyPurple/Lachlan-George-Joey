---
layout: default
title: Supplementry Information
nav_order: 2


---

{: .fs-6 .fw-300 }

# Supplementry Information
{: .no_toc }

---

 A computer system without a graphical user interface, _GUI_ can seem daunting. The good news is, most, if not all modern distributions of Linux include a GUI.

The goal of this section is to explain and show you that navigating Linux through the _CLI_ (command-line interface) is not difficult. With enough practice, you may find that using the _CLI_ to navigate through a computer is sometimes easier and even quicker.

Using the CLI also introduces more functionalities that you may overlook while you use a _GUI_. To use the Linux _CLI_, you will use an application called the _terminal_. 

---

### Table of contents
{: .no_toc .text-delta }
* TOC
{:toc}

---

## ASCII Table

Linux directories behave similarly to folders. In the background, directories are actually a special type of file used to store information about other files. The Linux operating system controls the contents. Contents include name, permission, type, size, etc.

You can find the home directory for common users under `/home/`[_username_] and the directory for the _root user_ under `root`.
![ASKEE TABLE](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/ASKEE%20table.png?raw=true "ASCII Tabe")

---

## Operator being used

| Command         | Description                                                                                             |
| :--------       | :------------------------------------------------------------------------------------------------------ |
| `ls`            | "List" all visible files and folders in the current directory.                                          |
| `pwd`           | "Print working directory" shows your current directory location.                                        |
| `cd`            | "Change directory" to a specified directory or your home directory.                                     |
| `open`          | "Open" a specified file, application, or directory.                                                     |
| `clear`         | "Clear" your terminal screen.                                                                           |
| `exit`          | "Exits" a terminal or a terminal session.                                                               |
| `history`       | Lists a "history" of issued commands.                                                                   |
| **[Up Arrow]**  | Scrolls through most recent command.                                                                    |

![Note icon](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/icons/note.png?raw=true "Note"){: style="float: left" }
> **Note:** You can find the full information about a command by using the `man` command. The syntax is `man [command]`.

---

## What the back end looks like

Below is a list of some common Linux commands.
![Memory dump](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/Memory%20dump.png?raw=true "memorydump")

**Note**: This list is not exhaustive.


---


You now know how to open the terminal and input commands which allow you to navigate through your system. 

Now you are able to see files in your directories as well as your current directory, allowing you to easily navigate through your system.

The next step is to learn how to [create users and assign privileges.](https://dl90.github.io/linux-basics/docs/users)
