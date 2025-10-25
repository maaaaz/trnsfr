trnsfr
======

Description
-----------
A simple Python script to upload files on transfer.sh servers from CLI.


Usage
-----
```
$ pip install trnsfr

$ trnsfr
usage: trnsfr.py [-h] [-s SERVER] [-i] [-k MAX_DAYS] [-t MAX_DOWNLOADS] [-d] [-v | -n | -q] [-e ENCRYPT_PASSWORD]
                 [-m {clamav,virustotal}]
                 file [file ...]

version: 1.2

positional arguments:
  file                  File(s) to upload

options:
  -h, --help            show this help message and exit

Connection parameters:
  -s, --server SERVER   Server instance URL (default: "https://transfer.adminforge.de/")
  -i, --ignore-tls-errors
                        Ignore TLS validation errors (default: False)

Upload parameters:
  -k, --max-days MAX_DAYS
                        Maximum number of days to keep file on the server
  -t, --max-downloads MAX_DOWNLOADS
                        Maximum number of times that file can be downloaded

Output parameters:
  -d, --show-delete-url
                        Show URL to delete (default: False)

Display parameters:
  -v, --verbose         Verbose output (default: False)
  -n, --no-progress-bar
                        Do not display the progress bar (default: False)
  -q, --quiet           Display only the download link without progress bar (default: False)

Confidentiality parameters:
  -e, --encrypt-password ENCRYPT_PASSWORD
                        Encrypt file with that password on the server-side (default: None)

Malware scan parameters:
  -m, --scan-malware {clamav,virustotal}
                        Scan for malware with ClamAV or Virustotal (default: None): /!\ this feature can be
                        unavailable on the server and hence failing the whole upload !
```
  

Credits
-------
* https://github.com/dutchcoders/transfer.sh
* https://github.com/tanrax/transfersh-cli


Copyright and license
---------------------

trnsfr is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

trnsfr is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  

See the GNU Lesser General Public License for more details.

You should have received a copy of the GNU General Public License along with trnsfr. 
If not, see http://www.gnu.org/licenses/.

Contact
-------
* Thomas Debize < tdebize at mail d0t com >