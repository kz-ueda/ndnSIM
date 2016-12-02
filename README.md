ndnSIM
======

[![Build Status](https://travis-ci.org/named-data-ndnSIM/ndnSIM.svg)](https://travis-ci.org/named-data-ndnSIM/ndnSIM)

A new release of [NS-3 based Named Data Networking (NDN) simulator](http://ndnsim.net/1.0/)
went through extensive refactoring and rewriting.  The key new features of the new
version:

- Packet format changed to [NDN Packet Specification](http://named-data.net/doc/ndn-tlv/)

- ndnSIM uses implementation of basic NDN primitives from
  [ndn-cxx library (NDN C++ library with eXperimental eXtensions)](http://named-data.net/doc/ndn-cxx/)

- All NDN forwarding and management is implemented directly using source code of
  [Named Data Networking Forwarding Daemon (NFD)](http://named-data.net/doc/NFD/)

- Allows [simulation of real applications](http://ndnsim.net/2.1/guide-to-simulate-real-apps.html)
  written against ndn-cxx library

[ndnSIM documentation](http://ndnsim.net)
---------------------------------------------

For more information, including downloading and compilation instruction, please refer to
http://ndnsim.net or documentation in `docs/` folder.

# Installation Procedure

The installation procedure is straight-forward and similar to the one of [ndnSIM](http://ndnsim.net/2.1/getting-started.html):

```bash
  # Download sources from github
  mkdir ndnSIM
  cd ndnSIM
  git clone https://github.com/schneiderklaus/ns-3-dev.git ns-3
  git clone -b pcon --recursive https://github.com/schneiderklaus/ndnSIM.git ns-3/src/ndnSIM

  # Compile and install 
  cd <ns-3-folder>
  make configure 
  make

```

