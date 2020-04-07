# Code Statistics

Rails provides us with the rake task `stats` to see code statistics within our application.

```
$ rails stats
+----------------------+--------+--------+---------+---------+-----+-------+
| Name                 |  Lines |    LOC | Classes | Methods | M/C | LOC/M |
+----------------------+--------+--------+---------+---------+-----+-------+
| Controllers          |     53 |     43 |       2 |       8 |   4 |     3 |
| Helpers              |     15 |     14 |       0 |       2 |   0 |     5 |
| Jobs                 |      7 |      2 |       1 |       0 |   0 |     0 |
| Models               |     40 |     29 |       2 |       5 |   2 |     3 |
| Mailers              |      4 |      4 |       1 |       0 |   0 |     0 |
| Channels             |      8 |      8 |       2 |       0 |   0 |     0 |
| JavaScript           |     28 |      8 |       0 |       0 |   0 |     0 |
| Libraries            |      0 |      0 |       0 |       0 |   0 |     0 |
| Controller tests     |      7 |      3 |       1 |       0 |   0 |     0 |
| Helper tests         |      0 |      0 |       0 |       0 |   0 |     0 |
| Model tests          |      7 |      3 |       1 |       0 |   0 |     0 |
| Mailer tests         |      0 |      0 |       0 |       0 |   0 |     0 |
| Channel tests        |     11 |      3 |       1 |       0 |   0 |     0 |
| Integration tests    |      0 |      0 |       0 |       0 |   0 |     0 |
| System tests         |      0 |      0 |       0 |       0 |   0 |     0 |
+----------------------+--------+--------+---------+---------+-----+-------+
| Total                |    180 |    117 |      11 |      15 |   1 |     5 |
+----------------------+--------+--------+---------+---------+-----+-------+
  Code LOC: 111     Test LOC: 6     Code to Test Ratio: 1:0.1
```
