cut provides to ways to define what "column" is.

- cut by field (-f) when the input consists of string (filed) each separated by single tab character

```bash
# print only 1 column from file
cut -f1 animals.txt
python
snail
alpaca
robin
horse
donkey
oryx

# print only 2 column from file
cut -f2 animals.txt
Programming Python
SSH, The Secure Shell
Intermediate Perl
MySQL High Availability
Linux in a Nutshell
Cisco IOS in a Nutshell
Writing Word Macros

# print 1 and 2 column from file
cut -f1-2 animal.txt  # print column 1 and 2
python	Programming Python
snail	SSH, The Secure Shell
alpaca	Intermediate Perl
robin	MySQL High Availability
horse	Linux in a Nutshell
donkey	Cisco IOS in a Nutshell
oryx	Writing Word Macros

# print 1 and 2 column and first 3 rows only from file
cut -f1-2 animals.txt | head -n3
python	Programming Python	2010
snail	SSH, The Secure Shell	2005
alpaca	Intermediate Perl	2012.
```

- cut by character position (-c)

```bash
# print first three character of each line
cut -c1-3 animals.txt
pyt
sna
alp
rob
hor
don
ory

# print authors last names
cut -f4 animals.txt | cut -d, -f1 
# here -d is delimiter changing seperator chacter to a comma instead of a tab
Lutz
Barrett
Schwartz
Bell
Siever
Boney
Roman
```
