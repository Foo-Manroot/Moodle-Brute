# Moodle-Brute [![Codacy Badge](https://api.codacy.com/project/badge/Grade/274ed0779e444337aff77062bd84eac0)](https://www.codacy.com/app/seymour_sec/Moodle-Brute?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Seymour-Sec/Moodle-Brute&amp;utm_campaign=Badge_Grade)
## Features
Brute force the moodle login page with a known username and a list of potential passwords, work is divided across multiple threads.

## Coming Soon
* Allow username lists
* Display progress better
* Increase efficiency

```
    __  ___             ____      ___           __
   /  |/  /__  ___  ___/ / /__   / _ )______ __/ /____
  / /|_/ / _ \/ _ \/ _  / / -_) / _  / __/ // / __/ -_)
 /_/  /_/\___/\___/\_,_/_/\__/ /____/_/  \_,_/\__/\__/
 Moodle Login Brute Forcer - Use with responsibility and within the law >.>
 by @Seymour_Sec

usage: moodleBrute [-h] [-v] -u URL -l LOGIN -p PASSWORD [-t THREADS]
                   [-D DELAY] [-s STATUS]

Moodle Login Brute Forcer

optional arguments:
  -h, --help            show this help message and exit
  -v, --version         prints version information
  -u URL, --url URL     the URL to moodle base install
  -l LOGIN, --login LOGIN
                        the username to try passwords for
  -p PASSWORD, --password PASSWORD
                        password list file
  -t THREADS, --threads THREADS
                        number of threads to use. default: 2
  -D DELAY, --delay DELAY
                        request delay (ms). default: 25
  -s STATUS, --status STATUS
                        status string returned by the server on UNSUCCESSFUL
                        attempts. default: "You are not logged in"
```
## Example Usage
`./moodleBrute.py -u http://target.com -l admin -p passwords`

*Use with responsibility, do not break the law.*
