# How to add flutter to path in mac parmanently
1: source ~/.zsh_profile
2: export PATH="$PATH:[NEW_DIRECTORY]/bin"
N/B: add your flutter path to the directory
3: Use command to save




#How to seperate text in textfield
With this keyboardType
keyboardType: TextInputType.number,
and with these inputFormatters inside the TextFormField Widget
// somewhere inside the code define the separator
var separator = ' - ';

[...]

// and add this to your `TextFormField` Widget
inputFormatters: [
                  /// allows card number length of 18 and 4 separators
                  LengthLimitingTextInputFormatter(18 + separator.length * 4),
                  CardFormatter(separator: separator),
                ],
