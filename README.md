SRPM tools for OpenSSH for RHEL 6 based operating systems
=========================================================

RHEL 6 is obsolete, but some people still use it. OpenSSH has new encryption protocols and has discarded some. This is a publicly tweaked, "mock" compatible build suite based on"

     http://rnd.rajven.net/centos/6/os/SRPMS/openssh-6.4p1-1cnt6.1.src.rpm

This github repo includes tools for building RPMs. "make" options
include:

  * make getsrc # Download the source tarballs
  * make build # Build with all docs and tests
  * make fastbuild # Build without docs and tests for fast smoke test

  * make # Build full multi-platform versions with mock
  * make install # build and install multi-platform versions in REPOBASEDIR

Run the "make getsrc" command, and run "make build" to build a local RPM under
rpmbuild.

Run "make" to use "mock" to build the default designated RPM's in the
local working directories such as epel-7-x86_64 and epel-6-x86_64.

       	  Nico Kadel-Garcia <nkadelgmail.com>
