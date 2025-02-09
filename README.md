# Reqs

- Php
- Node js(v.10 or above)
- Composer

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

Next, you need to install all project`s dependencies.
```
composer install
```

## Defining your enviroment

Create `.env` file and paste to it contents of `.env.example`.
Change variables(uncomment ones that are commented)
- DB_CONNECTION=mysql
- DB_HOST=`name-of-project`s root directory`-mysql-1
- DB_PORT=3306
- DB_DATABASE # your preferincies
- DB_USERNAME # your preferincies
- DB_PASSWORD # your preferincies

Launch server via sail. Flag `-d` makes container not binded to your tty.
```
./vendor/bin/sail up -d
```

## Launching npm client

To render your frontend, you need to run npm client.
```
npm run dev
```

# Closing server

To close your server use sail down command:
```
./vendor/bin/sail down
```
