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

