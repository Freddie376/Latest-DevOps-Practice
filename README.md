Part 1: Colors and basic listing (1-12)
1	ls	Lists the files and folders in the current folder.
2	ls --color=no	Lists them with no colors.
3	ls --color=yes	Lists them with colors, always.
4	ls --color=auto	Uses colors only when the output is shown on the screen. This is the usual default.
5	clear	Cleans the terminal screen.
6	ls -l	Long format. Shows permissions, owner, group, size, date and name for each item.
7	ls -n	Like -l, but shows the owner and group as numbers (IDs) instead of names.
8	ls	Back to the plain list.
9	ls -a	Shows all files, including hidden ones (names starting with a dot), plus . and ...
10	ls .	Lists the current folder. The . means "here".
11	ls -A	Like -a, but leaves out . and ...
12	ls -al	Long format and hidden files together.

Part 2: Times and creating files (13-25)
13	date	Shows the current date and time.
14	ls -lt	Long format, sorted by modification time (when the file content last changed). Newest first.
15	ls -ltu	Same, but uses the access time (when the file was last opened or read).
16	ls -ltc	Same, but uses the change time (when the file or its details, like permissions, last changed).
17	touch theNewestFile	Creates an empty file called theNewestFile. If it already exists, it only updates its time.
18	ls -ltu	Checks the access times again after creating the file.
19	ls -ltc	Checks the change times again.
20	echo "hello world!" > file-02	Writes the text "hello world!" into file-02. The > creates the file or replaces what was inside.
21	ls -ltu	Checks access times after writing.
22	ls -ltc	Checks change times after writing.
23	chmod 444 file-01	Changes permissions so file-01 is read-only for everyone (4 means read).
24	ls -ltu	Checks access times after the permission change.
25	ls -ltc	Checks change times. Changing permissions updates the change time, but not the modification time.

Part 3: File sizes (26-30)
26	ls -s	Shows the size of each file (in blocks) next to its name.
27	ls -ls	Long format plus the size in blocks.
28	ls -lh	Long format with human-readable sizes like K, M, G (based on 1024).
29	ls -l --si	Same idea, but sizes are based on 1000 instead of 1024.
30	ls -lSh	Sorts by size, largest first, with readable sizes.

Part 4: Output style (31-37)
31	ls -1	Shows one item per line.
32	ls -m	Shows items in one line, separated by commas.
33	ls -lQ	Long format with names inside double quotes.
34	ls -l	Back to normal long format.
35	ls -l --time-style=locale	Shows dates in the style of your system language and region.
36	ls -l --time-style=iso	Shows dates in short ISO style (year-month-day).
37	ls -l --time-style=full-iso	Shows the full date with seconds and time zone.

Part 5: More details and sorting (38-43)
38	ls -al --author	Adds a column for the file's author. On Linux this is usually the same as the owner.
39	ls -ald	The -d shows info about the folder itself, not what is inside it.
40	ls -ali	The -i shows each file's inode number (its unique ID in the system).
41	ls -alR	The -R is recursive: it also lists everything inside subfolders.
42	ls -alr	The -r reverses the order of the list.
43	ls -alSr	Sorts by size and reverses it, so the smallest files come first.

Part 6: Help and history (44-46)
44	ls --version	Shows which version of ls is installed.
45	ls --help	Shows a short guide to all ls options.
46	history	Shows the list of commands you typed before. This list came from it.

Quick option cheat sheet
-l	Long format (details)
-a / -A	Show hidden files (-A skips . and ..)
-h	Human-readable sizes
-t	Sort by time, newest first
-S	Sort by size, largest first
-r	Reverse the order
-R	Include subfolders
-d	Show the folder itself, not its contents
-i	Show inode numbers
-1	One item per line

Three times to remember
•	Modification time (ls -lt): when the content last changed.
•	Access time (-u): when the file was last read.
•	Change time (-c): when the file or its details (like permissions) last changed.
