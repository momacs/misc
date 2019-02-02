# Miscellaneous

## 1. `momacs` command-line utility
The [`momacs`](bin/momacs) utility alleviates the pain of performing common and often long, repetitive, and error-prone tasks (e.g., downloading the latest versions of [PRAM](https://github.com/momacs/pram)).  Currently supported operating systems are: FreeBSD, MacOS, and Ubuntu.

### 1.1. Installing
#### Prerequisites
First, make sure you have `curl` and `git` installed on your system.  You're set on MacOS.  On FreeBSD, do:
```
sudo pkg install -y curl git
```

On Ubuntu, do:
```
sudo apt install -y curl git
```

#### Install
To download the utility and make it executable, run the following commands:
```
mkdir -p ~/bin
cd ~/bin
curl -s -o momacs https://raw.githubusercontent.com/momacs/misc/master/bin/momacs
chmod u+x momacs
```

To add the `~/bin` to the PATH (and to have that change reflected in the current terminal session), run:
```
echo 'export PATH=$PATH:~/bin' >> ~/.bashrc
source ~/.bashrc
```

### 1.2. Using
To see the list of available commands, simply invoke it:
```
momacs
```

### 1.3. Updating
To check if a more up-to-date version is available in this repository, and to automatically download it, do:
```
momacs self update
```

If update is warranted, the current local version will be retained to enable rollback.  All retained previous versions can be removed like so:
```
momacs self remove-old-versions
```
