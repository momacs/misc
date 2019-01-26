# Miscellaneous

## `momacs` command-line utility
The [`momacs`](bin/momacs) utility alleviates the pain of performing common and often long, repetitive, and error-prone tasks (e.g., downloading the latest versions of [PRAM](https://github.com/momacs/pram)).

### Installing
To download the utility and make it executable, run the following commands:
```
mkdir -p ~/bin
cd ~/bin
curl -s -o momacs https://raw.githubusercontent.com/momacs/misc/master/bin/momacs
chown a+x momacs
```

Make sure `~/bin` is in your $PATH (`echo $PATH`).  If it is not there and if you are using the `bash` shell (default on MacOS and Ubuntu), do:
```
echo 'export PATH=$PATH:~/bin' >> ~/.bashrc
```

### Using
To see the list of available commands, simply invoke it:
```
momacs
```

### Updating
To check if a more up-to-date version is available in this repository, and to automatically download it, do:
```
momacs self update
```
