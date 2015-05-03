acd_cli install
===============

## Getting Started

You need `python3` to be installed. Get it from [https://www.python.org](https://www.python.org) or your favourite package manager.
In a terminal window type:

> Linux Ubuntu
    apt-get install python3
    apt-get install python3-pip

> Mac OS X (homebrew)
    brew install python3

*Hint:* Make sure if you currently are using `python2.X` that your bash/shell environment variable `${PYTHONPATH}` does not contain `python2.X` references.

Next you want to install the required dependencies. Using `pip3` is recommended to accomplish this:

    pip3 install --upgrade pip
    pip3 install sqlalchemy
    pip3 install python-dateutil
    pip3 install requests
    pip3 install pycurl
    pip3 install urllib3

### Download acd_cli

> Stable Release versions:
    https://github.com/cloud-drive/acd_cli/releases

> Latest Development version:
    https://github.com/yadayada/acd_cli/archive/master.zip

> git clone:
    git clone https://github.com/yadayada/acd_cli.git

### Initializing acd_cli

Now you can run `./acd_cli.py sync`, which will initiate the ACD authentication request from the main `acd_cli` folder.
This will open a browser window, which allows you to authenticate `acd_cli_oa` to access your Cloud Drive.
It may trigger a download of a file called `oauth_data.html` containing various `tokens`.

Place this file (`oauth_data.html`) into the main `acd_cli` folder and rename it to `oauth_data` (remove the extension).

Now press any key to continue to sync the directory structon from ACD. If you have a large amount of files, this may take a while.