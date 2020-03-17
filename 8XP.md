# #] This table is the token map for TI-Connect \*.8xp files only.

### #] Notices
1. Do not write `0001` for `▶DMS` all the time, TI-Connect checks if the `01` token is valid *first*, and if it 
is valid, writes `▶DMS`. For example: Writing `0102` in the hex editor will put `▶DMS▶Dec` in the TI Editor. Aditionally, 
you will see a couple bytes at `0x00000046` and `0x00000048`, the former is the total byte count and the latter is the program
token count. The difference between the two will end up at the end of the file and is the the checksum, but I don't know 
how to calculate that yet.

2. Several tokens will change their name if you change the language. Please choose `English` as your language on
when available if you want to verify this table.

3. Some of these tokens may change from calculator to calculator. For example, `Output(` on Z80 based calcs [eg TI82-4] is 
`Output ` on 68k based calcs [eg TI89-92].

4. Control characters when exported alone can allow you to view RAM, but back up your calc before viewing it, you may have to
reset it.

5. Different languages have different visuals, for example the `Å å Ø ø` tokens are only accessable in the svenska language,
but they map to `Â â Ô ô` respectively. Very annoying, I know.

### #] Keys
| Symbol | Meaning | Color |
| ------:|:------- | -----:|
| <+>    | Token prevents TI-Connect from opening the file, but it can be exported | Green |
| </>    | Token cannot be exported | Invis red |
| <!>    | Control character | Yellow |
| <?>    | Token breaks something [eg views RAM or breaks checksum] | Orange |

# #] Token index
Due to GitHub file size limits, I cannot post the table here. View it in [Google Sheets](https://docs.google.com/spreadsheets/d/1Q5f8AEPr1HTZEIx-dcEX2N4_G2LipvcRg33c17OfHgk/edit?usp=sharing) instead.
