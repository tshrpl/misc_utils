


# hexpng

<details>
<summary>figuring out the structure of a png file</summary>

```
89 50 4e 47 0d 0a 1a 0a| 00 00 00 0d 49 48 44 52  |.PNG........IHDR|
00 00 01 90 00 00 00 c8  08 02 00 00 00 49 77 20  |.............Iw |
b5|00 00 01 51 49 44 41  54 78 9c ed c3 21 01 00  |....QIDATx...!..|
00 08 c0 b0 f7 2f 0d 16  8f 9d 58 53 00 00 00 00  |...../....XS....|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 57 53 00 00 00 00  |..........WS....|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  |................|
00 00 00 00 1f 0b bb 7b  59 ba 2c 9e 77 6f|00 00  |.......{Y.,.wo..|
00 00 49 45 4e 44 ae 42  60 82|                   |..IEND.B`.|



signature:

89 50 4e 47 0d 0a 1a 0a |.PNG....|




IHDR:

00 00 00 0d       49 48 44 52
-----------       -----------
data length (13)  IHDR



89 50 4e 47 0d 0a 1a 0a| 00 00 00 0d_49 48 44 52  |.PNG........IHDR|
00 00 00 03_00 00 00 02__08_02_00_00_00_12 16 f1  |................|
4d|00 00 00 15_49 44 41  54_78 9c 6d c1 01 0d 00  |M....IDATx.m....|
00 00 40 30 fd 4b 53 c0  8e 2f 8f 88 0b f5_ec 04| |..@0.KS../......|
0e ce|00 00 00 00 49 45  4e 44 ae 42 60 82        |......IEND.B`.|




89504e470d0a1a0a0000000d49484452000000030000000208020000001216f14d0000001549444154789c6dc1010d0000004030fd4b53c08e2f8f880bf5ec040ece0000000049454e44ae426082



789c 6dc1010d0000004030fd4b53c08e2f 8f880bf5
789c 63f8cf80150200                 8f880bf5

01100100 01000011 01101111 01100100 01100101 00100000 10000011 01100011
10000010 01100101 01110011 00100000 01001100 01011010 01010111


00ff00ff 00ff00ff 00ff00ff 00ff00ff 00ff00ff 00ff00ff





89 50 4e 47 0d 0a 1a 0a| 00 00 00 0d 49 48 44 52_ |.PNG........IHDR|
00 00 00 03_00 00 00 02__08_02_00_00_00_12 16 f1  |................|
4d|00 00 00 18_49 44 41  54_78 9c 6d c3 31 01 00  |M....IDATx.m.1..|
00 00 c2 20 fb 47 22 9d  05 76 30 94 03 9d 08 0d  |... .G"..v0.....|
15_41 71 da 23|00 00 00  00 49 45 4e 44 ae 42 60  |.Aq.#....IEND.B`|
82                                                |.|

data:
789c6dc33101000000c220fb47229d05763094039d080d15




89 50 4e 47 0d 0a 1a 0a  00 00 00 0d 49 48 44 52  |.PNG........IHDR|
00 00 00 03 00 00 00 02  08 02 00 00 00 12 16 f1  |................|
4d|00 00 00 18_49 44 41  54_78 9c 6d c3 31 01 00  |M....IDATx.m.1..|
00 00 c2 20 fb 47 21 a5  05 76 30 94 03 8f 88 0b  |... .G!..v0.....|
f5_4e c2 bf 84|00 00 00  00 49 45 4e 44 ae 42 60  |.N.......IEND.B`|
82                                                |.|

file: 89504e470d0a1a0a0000000d49484452000000030000000208020000001216f14d0000001849444154789c6dc33101000000c220fb4721a505763094038f880bf54ec2bf840000000049454e44ae426082

data:
from file -> 789c6dc33101000000c220fb4721a505763094038f880bf5
decompressed -> 00aaaaaa 00aaaaaa 00aaaaaa 00aaaaaa 00aaaaaa 00aaaaaa






[ probably a correct attempt ]

89 50 4e 47 0d 0a 1a 0a| 00 00 00 0d_49 48 44 52_ |.PNG........IHDR|
00 00 00 03_00 00 00 02_ 08_02_00_00_00_12 16 f1  |................|
4d|00 00 00 19_49 44 41  54_78 9c 45 c6 31 0d 00  |M....IDATx.E.1..|
00 00 83 b0 f9 97 32 95  5c 84 5e dd d5 00 77 9c  |......2.\.^...w.|
0b f5_4c 78 3b 32|00 00  00 00 49 45 4e 44 ae 42  |..Lx;2....IEND.B|
60 82                                             |`.|

data:
from file -> 789c45c6310d00000083b0f99732955c845eddd500779c0bf5
decompressed -> 00 aaaaaa aaaaaa aaaaaa 00 aaaaaa aaaaaa aaaaaa





89 50 4e 47 0d 0a 1a 0a| 00 00 00 0d_49 48 44 52_ |.PNG........IHDR|
00 00 00 03_00 00 00 02_ 08_06_00_00_00_9d 74 66  |..............tf|
1a|00 00 00 0a_49 44 41  54_63 78 ad ac 5c 0f c3  |.....IDATcx..\..|
28 1c 00_ad e4 1e 3b|00  00 00 00 49 45 4e 44 ae  |(.....;....IEND.|
42 60 82                                          |B`.|


6378adac5c0fc3281c00





[ working ]

89 50 4e 47 0d 0a 1a 0a| 00 00 00 0d_49 48 44 52_ |.PNG........IHDR|
00 00 00 03_00 00 00 02_ 08_06_00_00_00_9d 74 66  |..............tf|
1a_00 00 00 10_49 44 41  54_78 da 63 78 ad ac 5c  |.....IDATx.cx..\|
0f c3 28 1c 00 87 86 0a  21_2f 6e ba 75|00 00 00  |..(.....!/n.u...|
00 49 45 4e 44 ae 42 60  82                       |.IEND.B`.|

data:
from file -> 78da6378adac5c0fc3281c0087860a21
data -> [0, 235, 35, 35, 127, 235, 35, 35, 127, 235, 35, 35, 127, 0, 235, 35, 35, 127, 235, 35, 35, 127, 235, 35, 35, 127]





```
</details>



