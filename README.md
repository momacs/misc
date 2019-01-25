# Miscellaneous

## `momacs` command-line utility
The [`momacs`](bin/momacs) utility alleviates the pain of performing common and often long and repetitive tasks (e.g., downloading the latest versions of [PRAM](https://github.com/momacs/pram)).

### Installing
To download the utility and make it executable do:
```
mkdir -p ~/bin
cd ~/bin
curl -s https://raw.githubusercontent.com/momacs/misc/master/bin/momacs
chown a+x momacs
```

If `~/bin` is not currently in your $PATH, you need to add it there:
```
echo "export PATH=$PATH:~/bin" >> ~/.bashrc
```

To see the list of available commands, invoke it like so:
```
momacs
```
