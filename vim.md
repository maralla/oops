Install latest vim in Ubuntu with clipboard support
===================================================

This is the steps to install vim from source and pretend to compile with python2 support.

```bash
$ sudo apt install libpython2.7-dev
$ sudo apt build-dep vim
$ git clone https://github.com/vim/vim.git
$ cd vim
$ ./configure --enable-pythoninterp=yes --enable-cscope --disable-netbeans --with-x --enable-terminal --enable-multibyte --with-python-command=python
$ make
$ sudo make install
```
