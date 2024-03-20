## Requirements

Python = 3.12.0  
Django = 5.0.3  
Tailwindcss

## Install Python

[Python.org](<[text](https://www.python.org/downloads/release/python-3122/)>)

Linux: [Python 3.12.2 Gzipped source tarball](https://www.python.org/ftp/python/3.12.2/Python-3.12.2.tgz)  
Linux: [Python 3.12.2 XZ compressed source tarball](https://www.python.org/ftp/python/3.12.2/Python-3.12.2.tar.xz)

macOS: [macOS 64-bit universal2 installer](https://www.python.org/ftp/python/3.12.2/python-3.12.2-macos11.pkg)

Windows: [Windows installer (64-bit)](https://www.python.org/ftp/python/3.12.2/python-3.12.2-amd64.exe)  
Windows: [Windows installer (ARM64)](https://www.python.org/ftp/python/3.12.2/python-3.12.2-arm64.exe)  
Windows: [Windows installer (32-bit)](https://www.python.org/ftp/python/3.12.2/python-3.12.2.exe)

## Check Python version

The following instructions will be for Linux terminals.

```bash
python3 -V' or 'python3 --version
```

## Clone Github directory

Github: [@stompsy/ccrp](https://github.com/stompsy/ccrp)

[HTTPS](https://github.com/stompsy/ccrp.git)  
[SSH](git@github.com:stompsy/ccrp.git)  
[GitHub CLI](gh repo clone stompsy/ccrp)

## Create virtual Python environment

Navigate to working directory (i.e. _ccrp_) and then run the following command. The following command will place a directory called _venv_ in your working directory:

```bash
python3 -m venv venv
```

Then activate your virtual environment (from the same working directory):

```bash
source venv/bin/activate
```

## Install dependencies

To install Python environment requirements:

```bash
pip install -r requirements.txt
```

Install Tailwindcss requirements:

```bash
npm install -D tailwindcss #You do not need to initialize tailwindcss as a basic configuration file has already been generated.
```

## Run development server & Tailwindcss watch script

From the _src_ directory, or wherever your _manage.py_ file is located, run:

```bash
python manage.py runserver
```

You should see something like:

```bash
Django version 5.0.3, using settings 'gdnhome.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
```

From the root directory, i.e. _ccrp/_, run:

```bash
npm run dev
```

You should see something like:

```bash
tailwindcss -i src/static/tw/tailwind-input.css -o src/static/css/gdnhome-ui.css --watch

Rebuilding...

Done in 229ms.
```

Thanks for playing!
