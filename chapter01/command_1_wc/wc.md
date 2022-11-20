```bash
wc animals.txt
7 51 325 animals.txt
## wc reports that file animals.txt has 7 lines, 51 words and 325 characters

wc -l animals.txt
7 animals.txt

wc -w animals.txt
51 animals.txt

wc -c animals.txt
325 animals.txt

wc animals.txt | wc
4
## wc animals stdout to wc i.e 7 51 325 animals.txt | wc
### which gives 3 integer and a file name = 4

wc animals.txt | wc -w | wc
1    1    2
## 1 word 1 line 2 character (4 ends with invisible new line character)
```
