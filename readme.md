# datebook

A tiny datebook script.

## Installation

```bash
git clone https://github.com/havenwood/datebook.git
cd datebook
gem i -g
```

## Usage

```
Usage: datebook [DATE_OR_TIME]
    -r, --remove   specify date or time of event to remove
    -l, --list     list all events
    -h, --help
    -v, --version
```

## Examples

Creating calendar entries:
```bash
./datebook next tues at 2:15pm
#>> Tue, May 19 at 02:15pm
#>> Event: ...

./datebook tues evening
#>> Tue, May 19 at 06:30pm
#>> Event: ...
```

Listing calendar entries:
```bash
./datebook --list
#>> Tue, May 19 at 02:15pm: Brunch!
#>> Tue, May 19 at 06:30pm: After brunch.
```

Removing calendar entries:
```bash
./datebook --remove Tues at 2:15 PM
#>> Removing event on Tue, May 19 at 2:15pm:
#>> 	Brunch!
#>> Event successfully removed.
```
