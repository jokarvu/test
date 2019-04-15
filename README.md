```
kienpnh@ptit:~$ sudo apt install postgresql
```

```
kienpnh@ptit:~$ sudo -u postgres createuser $USER
kienpnh@ptit:~$ sudo -u postgres psql -c "alter user $USER with superuser" postgres
```

```
kienpnh@ptit:~$ sudo -u postgres createuser canvas --no-createdb --no-superuser --no-createrole --pwprompt
kienpnh@ptit:~$ sudo -u postgres createdb canvas_production --owner=canvas
```

```
kienpnh@ptit:~$ sudo apt install apache2
```

```
kienpnh@ptit:~$ sudo add-apt-repository ppa:brightbox/ruby-ng
kienpnh@ptit:~$ sudo apt-get update
kienpnh@ptit:~$ sudo apt-get install ruby2.4 ruby2.4-dev zlib1g-dev libxml2-dev libsqlite3-dev \
                                     libpq-dev libxmlsec1-dev curl make g++
```

```
kienpnh@ptit:~$ sudo gem install bundler --version 1.13.6
kienpnh@ptit:~$ bundle _1.13.6_ install --path vendor/bundle
```

```
kienpnh@ptit:~$ curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
kienpnh@ptit:~$ sudo apt-get install nodejs
```
