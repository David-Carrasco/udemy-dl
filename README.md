A Python script to download lecture videos for a udemy.com course.

### Prerequisites

* Python (2 or 3)
* `pip` (Python Install Packager)
* Python modules `beautifulsoup4` and `requests`
  * If missing, they will be automatically installed by `pip`


### Preinstall

If you don't have `pip` installed, look at their [install doc](http://pip.readthedocs.org/en/latest/installing.html).
Easy install (if you trust them) is to run their bootstrap installer directly by using:

    sudo curl https://bootstrap.pypa.io/get-pip.py | python


### Install

`udemy-dl` can be installed using `pip`

    sudo pip install udemy-dl


### Usage

Simply call `udemy-dl` with the full URL to the course page.

    udemy-dl https://www.udemy.com/COURSE_NAME

`udemy-dl` will ask for your udemy username (email address) and password then start downloading the videos.

By default, `udemy-dl` will create a subdirectory based on the course name.  If you wish to have the files downloaded to a specific location, use the `-o /path/to/directory/` parameter.

If you wish, you can include the username/email and password on the command line using the -u and -p parameters.

    udemy-dl -u user@domain.com -p $ecRe7w0rd https://www.udemy.com/COURSE_NAME

For information about all available parameters, use the `--help` parameter

    udemy-dl --help


### Uninstall

`udemy-dl` can be uninstalled using `pip`

    sudo pip uninstall udemy-dl

You may uninstall the required `beautifulsoup4` and `requests` modules too but be aware that those might be required for other Python modules.
