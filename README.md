# WhiteTiger DDoS Tool

WhiteTiger is only a tool for SECURITY TESTING PURPOSES!

WhiteTiger is an HTTP DDoS Tool.

Attack Vector exploited: HTTP Keep Alive + NoCache

Warning: don't try with .edu and .gov

## Usage

```sh
git clone https://github.com/km2262488/white_tiger.git
cd whitetiger
python3 whitetiger.py --help
```

## Options

```sh
python3 whitetiger.py <url> <options>

Options            Description                                      Default
-u, --useragents   Type of user-agents to generate                  (default: randomly generated)
                   (see in http://www.useragentstring.com/)
-w, --workers      Number of concurrent workers to attack           (default: 50)
-s, --sockets      Number of concurrent sockets                     (default: 100)
-m, --method       HTTP Method to use                               (default: get)
                   (get/post/random)
-d, --debug        Enable Debug Mode (more verbose output)          (default: False)
                   (True/False)
-n, --nosslcheck   Do not verify SSL Certificate                    (default: True)
                   (True/False)
-h, --help         Shows this help

Example: python3 whitetiger.py https://example.com -w 1000 -s 1000 -m post
```

Check website monitoring in https://check-host.net/


## Utilities
   
* Added randomly created user agents (still RFC compliant).
* Added external user-agent list support.
* http://www.useragentstring.com/
* Increased worker and socket capacity.
* Changed from threading to multiprocessing.
* Improved randomness of referers.
* Added Debug Mode.
* Added support for not verifying SSL Certificates.


## License
This software is distributed under the GNU General Public License version 3 (GPLv3)

## LEGAL NOTICE
THIS SOFTWARE IS PROVIDED FOR EDUCATIONAL USE ONLY!
WARNING: DON'T TRY WITH .EDU AND .GOV
IF YOU ENGAGE IN ANY ILLEGAL ACTIVITY THE AUTHOR DOES NOT TAKE ANY RESPONSIBILITY FOR IT. 
BY USING THIS SOFTWARE YOU AGREE WITH THESE TERMS.
