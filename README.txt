google-libusb

Prerequisites:

  sudo apt-get install \
    libusb-1.0-0-dev \
    libgtest-dev \

  cd ~/Downloads
  wget http://gflags.googlecode.com/files/libgflags0_2.0-1_amd64.deb
  wget http://gflags.googlecode.com/files/libgflags-dev_2.0-1_amd64.deb
  wget http://google-glog.googlecode.com/files/glog-0.3.3.tar.gz
  sudo dpkg -i *.deb

  mkdir -p ~/src
  cd ~/src

  tar zxf ~/Downloads/glog-0.3.3.tar.gz
  cd ~/src/glog-0.3.3
  ./configure && make deb
  [ Type 'y' when it prompts to continue. ]
  sudo dpkg -i packages/debian-wheezy/sid/libgoogle-glog*.deb


