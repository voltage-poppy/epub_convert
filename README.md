# epub_convert
Online Version: https://epub.stoneapp.tech/

## Requirements
- Python 3.6 or newer

## Libraries
- Flask >= 0.13.0
- OpenCC
- TocasUI
- axios

## Usage
- command line
```bash
$ python convert.py <epub>
```

- development web server
```bash
$ python web.py
```

- apache `mod_wsgi`
```apache
<VirtualHost *:80>
    ServerName domain.name

    WSGIDaemonProcess appname user=user1 group=group1 threads=5
    WSGIScriptAlias / /location/to/folder/web.wsgi
    Alias /static /location/to/folder/static

    <Directory "/location/to/folder">
        Require all granted
    </Directory>
</VirtualHost>
```

## Installation


```shell
pip install git+https://github.com/voltage-poppy/epub_convert.git
```

or
```shell
uv tool install git+https://github.com/voltage-poppy/epub_convert.git
```

Two command line tools `epub-s2t` and `epub-t2s` will be available after installation.

To uninstall, run
```
pip uninstall epub-convert
```

or 
```
uv tool uninstall epub-convert
```
