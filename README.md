turnip
======

Use turnip to keep a personal log of when you work during the day. The main
use case is for hourly workers who spend a lot of time in the terminal.
Keeping a close eye on your hours ensures you're compensated for every bit of
time you work, or conversely motivates you to be more productive.


### Requirements

You'll need SQLite3 and sqlite3-ruby installed: `gem install sqlite3`. Is that
overkill for something as simple as this? The answer is yes.


### Usage

`turnip start` and `turnip stop` to punch in and out.

`turnip show` to print the entire log, `turnip show -n 5` to print the last
five days logged.

`turnip clear` to clear the log.

You can keep things in the log for as long as you like, but if you wish you
can easily archive the current records and start fresh by doing something like
`turnip show > week-01-hours.txt` followed by `turnip clear`.

Should you ever want to poke around the database manually, the default location
is `~/.turnip/intervals.db`.

### License
MIT
