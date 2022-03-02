brew install cmake ctags

PYTHON_CONFIGURE_OPTS="--enable-framework" \
    CPPFLAGS="-I$(brew --prefix openssl)/include -I$(brew --prefix libffi)/include" \
    LDFLAGS="-L$(brew --prefix openssl)/lib -L$(brew --prefix libffi)/lib" \
    pyenv install -v 3.9.9

PYTHON_CONFIGURE_OPTS="--enable-framework" \
    CPPFLAGS="-I$(brew --prefix openssl)/include -I$(brew --prefix libffi)/include" \
    LDFLAGS="-L$(brew --prefix openssl)/lib -L$(brew --prefix libffi)/lib" \
    pyenv install -v 3.10.1
# pyenv4mac

PYTHON_CONFIGURE_OPTS="--enable-framework" \
pyenv install 3.9.10
pyenv global 3.9.10
