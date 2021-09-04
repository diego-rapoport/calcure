# calcure

Minimal TUI calendar with stylish and customizable UI in linux terminal. You can add and edit events and view birthdays from your [abook](https://abook.sourceforge.io/) and import events from [calcurse](https://github.com/lfos/calcurse).

![screenshot](screen.jpeg)

## Features

- Vim keys
- Event management with a fewest key presses possible
- Birthdays from your abook contacts
- Auto pictograms according to event name ✈ ⛷ ⛱
- Privacy mode ••••• to obfuscate events
- Simple plain text database in a desired location for cloud sync
- Colors, icons, and other features are fully customizable
- Resize friendly. Can shrink to a small window
- Import from calcurse
- Start week on any day


## Instalation and running

Simply copy the **calcure** file into a directory with your binaries, for example into `home/user/.local/bin` 

Then, run by just typing `calcure` in a linux terminal.

In case of permission error, you'll need to make the file executable `chmod =rwx calcure`.

Also, it requires python 3 to run. If you don't have it, install `python` package from your standard repository.

## Key bindings

`n`,`j`,`l`,`↓` - next month

`p`,`h`,`k`,`↑` - previous month

`a`,`space` - add event

`A` - add recuring event

`e`,`c` - edit event

`d`,`x` - delete event

`home`,`gg`,`G` - return to current month

`i` - import events from calcurse

`*` - Toggle privacy mode

`?` - toggle footer

`q` - quit


## Configuration

On the first run, it will create a configuration file at `home/user/.config/calcure/config.ini`

You can edit parameters and colors in the `config.ini` file. Here is an example config:

```
[Parameters]
folder_with_datafile = /home/user/.config/calcure
birthdays_from_abook = Yes
show_keybindings = Yes
show_day_names = Yes
minimal_today_indicator = Yes
minimal_days_indicator = Yes
minimal_weekend_indicator = Yes
cut_titles_by_cell_length = Yes
privacy_mode = No
ask_confirmations = Yes
use_unicode_icons = Yes
start_week_day = 1
event_icon = •
today_icon = •
privacy_icon = •
birthday_icon = ★
hidden_icon = ...

[Colors]
color_today = 2
color_days = 7
color_day_names = 4
color_weekends = 1
color_weekend_names = 1
color_hints = 7
color_propmts = 7
color_birthdays = 1

[Diologs]
hint =  n: Next month · p: Previous month · a(A): Add (recurring) event · d: Delete · e: Edit · i: Import · q: Quit · ?: Help

[Event icons]
travel = ✈
plane = ✈
trip = ✈
voyage = ✈
flight = ✈
airport = ✈
vacation = ⛱
holyday = ⛱
day-off = ⛱
hair = ✂
barber = ✂
beauty = ✂
nails = ✂
game = ♟
match = ♟
play = ♟
interview = ♟
date = ♥
concert = ♪
gig = ♪
disco = ♪
music = ♪
rehersal = ♪
call = ☎
phone = ☎
deadline = ⚑
over = ⚑
finish = ⚑
end = ⚑
appointment = ✔
task  = ✔
doctor = ⛑
dentist = ⛑
medical = ⛑
hospital = ⛑
party = ☘
museum = ⛬
meet = ⛬
talk = ⛬
conference = ⛬
hearing = ⛬
sport = ⛷
gym = ⛷
training = ⛷
```
When configuring colors, the numbers mean: 1 - red, 2 - green, 3 - yellow, 4 - blue, 5 - magenta, 6 - cyan, 7 - white

