# saltstack
# soledad208
The original Saltstack Minion installtion package was built with libcurl 7.47, which crash on windows 64bit when using "proxy_host" and "proxy_port" options.
This customized version using libcurl 7.51, and tested on windows server 2012 R2.
INSTALLATION:
- Download and install customized saltstack minion setup
OR:
- Download and install original saltstack minion setup at: https://repo.saltstack.com/windows/Salt-Minion-2017.7.1-Py2-AMD64-Setup.exe
- Install customized pycurl setup and point to saltstack's python folder (default is: C:\salt\bin)
CHECK IF libcurl is 7.51:
Open cmd and run command:
  cd C:\salt\bin
  python
  import pycurl
  pycurl.version
Good output:
  'PycURL/7.43.0 libcurl/7.47.0 OpenSSL/1.0.2e zlib/1.2.8 c-ares/1.10.0 libssh2/1.6.0'

ENJOY!
