## Requirements

Python = 3.12.0  
Django = 5.0.3  
Tailwindcss

## Install Python

[Python.org](https://www.python.org/downloads/release/python-3122/)

Linux: [Python 3.12.2 Gzipped source tarball](https://www.python.org/ftp/python/3.12.2/Python-3.12.2.tgz)  
Linux: [Python 3.12.2 XZ compressed source tarball](https://www.python.org/ftp/python/3.12.2/Python-3.12.2.tar.xz)

macOS: [macOS 64-bit universal2 installer](https://www.python.org/ftp/python/3.12.2/python-3.12.2-macos11.pkg)

Windows: [Windows installer (64-bit)](https://www.python.org/ftp/python/3.12.2/python-3.12.2-amd64.exe)  
Windows: [Windows installer (ARM64)](https://www.python.org/ftp/python/3.12.2/python-3.12.2-arm64.exe)  
Windows: [Windows installer (32-bit)](https://www.python.org/ftp/python/3.12.2/python-3.12.2.exe)

## Check Python version

The following instructions are for Linux terminals.

```shell
python3 -V
# or
python3 --version
```

## Clone Github directory

HTTPS: **\https://github.com/stompsy/ccrp.git\**  
SSH: **\git@github.com:stompsy/ccrp.git\*\*  
GitHub CLI: **gh repo clone stompsy/ccrp**

## Create virtual Python environment

Navigate to the working directory (i.e. `ccrp/`) and then run the following command. The following command will place a directory called `venv` in your working directory:

```shell
python3 -m venv venv
```

Then activate your virtual environment (from the same working directory):

```shell
source venv/bin/activate
```

## Install dependencies

To install **Python** environment requirements:

```shell
pip install -r requirements.txt
```

Install **Tailwindcss** requirements:

```shell
npm install -D tailwindcss
#You do not need to initialize tailwindcss as a basic configuration file has already been generated.
```

## Run development server & Tailwindcss watch script

From the `src` directory, or wherever your `manage.py` file is located, run:

```shell
python manage.py runserver
```

You should see something like:

```shell
Django version 5.0.3, using settings 'gdnhome.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
```

From the root directory, i.e. `ccrp/`, run:

```shell
npm run dev
```

You should see something like:

```shell
tailwindcss -i src/static/tw/tailwind-input.css -o src/static/css/gdnhome-ui.css --watch

Rebuilding...

Done in 229ms.
```

Thanks for playing! :wave:
