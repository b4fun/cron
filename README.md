# cron

A visual cron.

## Usage

```
*/1 * * * * python myscript.py
```

in web app:

```
app: python myscript.py
output:
hello, world
```

### Apply new app

```
$ cat app-curl-google.yaml
app:
  name: curl google
  command:
    - curl
    - https://www.google.com
  schedule:
    hour: */4
```

```
$ cronctl apply -f app-curl-google.yaml
```
