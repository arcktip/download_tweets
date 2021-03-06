##Download Tweets

Download all the Tweets For a Twitter Username

### Author

* Author: Ryan McGreal
* Email: [ryan@quandyfactory.com](mailto:ryan@quandyfactory.com)
* Homepage: [http://quandyfactory.com/projects/48/download_tweets](http://quandyfactory.com/projects/48/download_tweets)
* Repository: [http://github.com/quandyfactory/download_tweets](http://github.com/quandyfactory/download_tweets)

### Licence

Released under the GNU General Public Licence, Version 2:

[http://www.gnu.org/licenses/old-licenses/gpl-2.0.html](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)

### This Version

* Version: 0.5.2

* Release Date: 2013-09-12

### Installation

It's pretty simple to install, assuming you have Python installed on your system. Linux and Mac OSX users have Python installed by default. Windows users will need to [download and install Python](http://python.org/download/) - install version 2.6.x, not version 3.

Once you have determined that you have Python on your system, just download the `download_tweets.py` script and save it somewhere.

It uses only the standard Python library with no additional third party dependencies.

### Using Download Tweets
    
#### Interactive Mode

To use Download Tweets interactively, just execute `download_tweets.py`. (*nix uses might have to set execute permissions.)

The script will prompt you to enter the Twitter username you want to download. Then it will download all of that user's tweets (see Note #1, below) and save them in a tab-delimited text file named `Tweets_*Username*.txt`. 

You should be able to open the data file in a spreadsheet program.

#### Non-interactive Mode

Thanks to an addition by [Jay Parlar](http://github.com/parlarjb/download_tweets), you can execute `download_tweets.py` with optional command line arguments:

    ./download_tweets.py -u Username -o Filename.txt

That's it.

## Notes

1. The twitter API will only let you [download the most recent 3,200 tweets](https://dev.twitter.com/docs/things-every-developer-should-know). (Don't worry - all your tweets are still in their database. They eventually plan to make them all available.)

2. The Twitter API also [limits the number of data requests](https://dev.twitter.com/docs/rate-limiting) to 150 per hour. 


### Revision History

### Version: 0.5.2

* Release Date: 2013-09-12
* Changes:
    * Fixed error in filename.

### Version: 0.5.1

* Release Date: 2013-04-08
* Changes: 
    * Fixed bug that caused line breaks in tweet text.

### Version: 0.5

* Releast Date: 2012-09-28
* Changes:
    * Filename now includes date/time stamp of when the script ran.

#### Version: 0.4

* Release Date: 2012-07-24
* Changes:
    * Better error handling, including passing error message from twitter server to console.

#### Version: 0.3

* Release Date: 2012-07-23
* Changes:
    * Changed JSON parsing and conversion to tab-delimited to track change in twitter API.

#### Version: 0.2

* Release Date: 2010-04-06
* Changes:
    * Merged fork from Jay Parlar that added option parsing for username and output filename.

#### Version: 0.1

* Release Date: 2010-03-31
* Changes:
    * First commit.
