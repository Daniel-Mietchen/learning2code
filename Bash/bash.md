# About

Some bash stuff that I found interesting/ useful.

# Special characters

## ```$```

* when called followed by a variable, e.g., ```$a```, it gives the current value of that variable

## ```.```

* shorthand for the current directory

## ```()```


## ```[]```


## ```{}```


# Bash commands

## ```enable```/ ```disable```

* allows to enable/ disable builtin shell commands

## ```compgen -k```

* lists the keywords used in bash

## ```source```

* imports variable assignments or functions
  - e.g. ```source test.sh``` would import variable assignments or functions from ```test.sh```

# Bash customization

* ```.bash_profile``` is executed upon login to the shell
  - usually used to set environment variables
    - e.g. ```PATH=$PATH:/usr/local/bin```
* ```bashrc``` is executed upon starting a new shell
  - typical use is to set aliases
