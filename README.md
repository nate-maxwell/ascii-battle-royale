# Ascii Battle Royale

This is a (very) simple terminal simulation of 192 characters battling it out to be the last one standing,
written in my own interpreted language [Silver](https://github.com/nate-maxwell/silver-lang).

Running the `main.slv` will begin the simulation. Upon starting there will be three copies of each of the
following characters:
```silver
[
  "A", "B", "C", "D", "E", "F", "G", "H",
  "I", "J", "K", "L", "M", "N", "O", "P",
  "Q", "R", "S", "T", "U", "V", "W", "X",
  "Y", "Z", "!", "@", "#", "$", "%", "^",
  "&", "*", "(", ")", "-", "=", "+", "~",
  "1", "2", "3", "4", "5", "6", "7", "8",
  "9", "0", "<", ">", "?", "[", "]", "\\",
  "{", "}", ";", ":", ".", ",", "`", "|"
]
```

A `cyan`, `magenta`, and `yellow` one will spawn.
* `cyan` characters move small distances
* `magenta` characters move moderate distances
* `yellow` characters move larger distances

When two characters collide, one of them survives.
The turn rate increases when there are 10 or fewer remaining characters.

The sim does not end with only one character remains, instead they will move around endlessly.

The battleground is determined by terminal size on program start. For best results, full screen
the terminal to get as many rows and columns for characters to occupy.

<img src="https://i.imgur.com/ZB6LMAw.png">
