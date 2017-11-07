# timestamp

Creates a nice ISO-8601 timestamp for usage in filenames, this is a built in 
format in some implementations of date.

## Installation
Put the script somewhere in you path, i.e. in $HOME/bin (only you)
or /usr/local/bin (everyone)
```sh
sudo cp template /usr/local/bin
```

## Usage
Add timestamp to a filename on a backup
```sh
cp file.ext /mnt/backup/file.$(timestamp).ext
```

Create a note with the current timestamp
```sh
vi meeting-notes-$(timestamp).txt
```

Just show the current timestamp
```sh
timestamp
```

### Only use the day
Sometimes you only want the day and not the full timestamp, for those cases I've
added the `day` option which can also be invoked with `-d` like below
```sh
$ timestamp day
2017-11-07
$ echo notes-$(timestamp -d).txt
notes-2017-11-07.txt
```

