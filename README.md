brew install cmake
cd ~/.vim
git clone https://github.com/Valloric/YouCompleteMe.git
mkdir YouCompleteMe/ycmbuild
cd YouCompleteMe/ycmbuild
cmake -G "Unix Makefiles" . /Users/tmihalicek/.vim/plugged/YouCompleteMe/third_party/ycmd/cpp
make ycm_core
Restart Vim
Enjoy
@RyanCarey
RyanCarey commented on 13 Mar 2018 •
I had to use
6. cmake -G "Unix Makefiles" . ~/.vim/bundle/YouCompleteMe/third_party/ycmd/cpp/
but otherwise this worked for me.


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
