# yubifun

## How to install
Using Pip

python-yubico is installable via pip:

$ pip install python-yubico

Or, directly from the source package in the standard Python way:

$ cd python-yubico-$ver
$ python setup.py install

This requires the python-setuptools package. You will also need PyUSB, called python-usb in Debian/Ubuntu. pyusb is available on PyPI and may be installed with pip: pip install --pre pyusb The --pre command-line option indicates that pre-releases of pyusb may also be searched (only pre-releases of pyusb are available on PyPI, and pip skips pre-releases by default). Note that while both the 0.4 branch and the 1.0 branch are supported, the older 0.4 branch doesn’t support re-attaching the kernel device driver on close, which will leave the YubiKey in a state where it is unable to output OTPs until it has been unplugged and plugged back in again.
On Windows

If you use Windows, you will require a PyUSB backend. Python-yubico has been tested with libusbx and confirmed working, without the need for replacing the device driver.
