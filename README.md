# Helpful Linux Commands (Debian)
Some Helpful commands for debian linux. I am completely unskilled in arch, however, so I do not have a guide for arch. There are collections of commands in the master branch. 

# Category One: Navigation
Whether the linux distro you are using is debian based or not, this will be the same. The basic Navigation Commands Are:
 - `ls`, to list the folders and files in your current directory, 
 - `cd`, to move to a new directory. e.g. `cd Desktop`

Most people are already familliar with those commands, however.
# Category Two: File Editing
- `nano` is a built-in text editor for most distros, but you can install it  with `sudo apt get nano -y`. Ex. `nano text.txt` will edit the file `text.txt` if it exists. If it dosen't, then it will create the file and edit it. The file must be in the same directory.
- `vi`, or `vim`, are more advanced editors, and do the same thing as `nano`. I would not recommend them, and you should use `nano` instead. if you would like to know how to use it, look it up on [vim.org](vim.org). 
- `touch` will create files, without editing them. Ex. `touch text.txt` will create `text.txt` as an empty file. 
# Category Three: Package management with apt and snapd
Apt is a package manager (with super cow powers), that installs packages with ease. 
> On Ubuntu, `snap` is an option as well. Snap will be talked about later.
 > 
 - an example of `apt` is: `sudo apt install chromium-browser`. Not all packages (apps) Have the same naming scheme
 - There are certain switches for apt, such as `-y`, which when appended to an install command will remove comfirmation to install. Ex. `sudo apt install chromium-browser` will ask for confirmation (y or N), and `sudo apt install chromium-browser -y` will automatically install with no confirmation. 
 - `apt list chrome` will search descriptions and titles for the word `chrome`, and show matching packages. It is very useful if you don't know the name of a package you want to install.
 - `apt` is also your update program. There's also `apt-get`, which does (on a simple level) the same thing as `apt`. It is considered a backend version, and has all of the same features, but `apt` is meant to be more for humans. If an installation guide asks to use `apt-get`, then it will do the same thing.
 >Side note: `apt` has a 3rd party gui, called `synaptic`. To install, use `apt install synaptic.`
 
- `apt full-upgrade` will update all of your packages to the latest version.
 - `apt update`  does NOT update packages, but rather repos, or the sources that the apps come from. 
 # Category Three Part Two: Snap
 `snap`, or `snapd`, is another package management software that comes with ubuntu. It works in the same way, and also comes with a gui. To install it on another distro, run `apt install snapd`.

-  `snap` works in the same way as `apt`, and has most of the same features. `apt` is still the best option for system updates, but `snap` has apps that `apt` dosen't, and vice versa. 
- The syntax for `snap` is `snap install <Package name>`, just like `apt.`

## That's the end of the tutorial! (so far)
The basic skills add up to this, and it isn't much, but that's the basics. If you know how to do stuff like this, your family will think you are a technician, especially if you're like 12 years old. That's it, so thanks for reading, and goodbye from MrMilk.