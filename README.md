# Reqs

- Php

# Installing

Firstly, clone repository to your machine

```
git clone https://github.com/mega-daun/pastebin
```

# Launching server via Docker container

Go to project directory

```
cd pastebin
```

Launch server via sail. Flag `-d` makes container not binded to your tty.
```
./vendor/bin/sail up -d
```

# Closing server

To close your server use sail down command:
```
./vendor/bin/sail down
```