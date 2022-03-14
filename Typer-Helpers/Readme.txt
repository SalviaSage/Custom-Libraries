Devanagari Typer Helper — Documentation

I created this Hotstrings.exe library to tackle an issue with typing vowels in the Devanagari script
and in other Indic scripts.

In the Devanagari alphabet, vowels can be written in 2 ways. The independent vowel forms and the maatra forms.
I assigned the vowel keys to type the maatra forms while pressing caps lock + vowel keys give us the independent vowel forms.

However, this makes it so that the maatras are also typed at the start of words where the independent vowel forms would be.
For example, you wanted to type उत्तर , but you got ुत्तार instead. This mistake would never be done if writing with a pen and paper.
But in this scenario it is done since the maatra and the independent vowels are treated as different letters by the computer.
At the start of words, the maatras would never be used. So, what this custom library does is that it automatically detects
and deletes the starting maatras and replaces them with their independent vowel forms.

There are twenty-three definitions here for tacking this problem and I like to think it is an indispensable program
for typing with the Devanagari script and the other Indic scripts that are affected by this problem.

This custom library is based on the program found here: https://github.com/mslonik/Hotstrings
I am not the author of this program and that program is in active development as of writing this.
