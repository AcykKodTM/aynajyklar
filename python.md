
# Mirror urls

[https://mirror-pypi.runflare.com/simple/](https://mirror-pypi.runflare.com/simple/)
[https://mirrors.aliyun.com/pypi/simple/](https://mirrors.aliyun.com/pypi/simple/)
[https://mirrors.ustc.edu.cn/pypi/simple/](https://mirrors.ustc.edu.cn/pypi/simple/)
[https://mirrors.sustech.edu.cn/pypi/web/simple](https://mirrors.sustech.edu.cn/pypi/web/simple)


# How to add
How to install package from mirror without adding it to the configuration.
To do that we use "-i" flag and giving a url of a mirror:

```bash
pip install <packages...> -i https://example-of-mirror.com/simple
```

If you don't to manually specifiy mirror for each time you download and want to 
just store one mirror then you can open pip configuration file.

### Local pip config
**MacOS/Linux**: $HOME/.config/pip/pip.conf
**Windows**: %APPDATA%\pip\pip.ini

Config file example
```
[global]
# index-url = <URL>
# index = <URL>


```

### Per virtual envrinment pip config
**MacOS/Linux**: $VIRTUAL_ENV/pip.conf
**Windows**: $VIRTUAL_ENV/pip.ini

### Set pip from command line
pip config --user set global.index <URL>
pip config --user set global.index-url <URL>



