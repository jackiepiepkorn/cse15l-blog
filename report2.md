# Lab Report 2

## Code Change 1
![Image 1](https://i.imgur.com/46loSbr.png)
This is the symptom

[Test File #1](https://github.com/jackiepiepkorn/cse15l-blog/blob/65caf524a5a2254b7675c08d014529b6a7b69dbe/test-file2.md)

The bug is that the program continues searching for links after there are no more links, which causes it to create the symptom of running out memory when the loop keeps running. The failure inducing input is the test-file2.md, which has a line after its links, which causes the for loop to keep going.

Here was my fix: ![Fixed Code](https://i.imgur.com/3MtAYKN.png)

</br>

## Code Change 2
![Image 2](https://i.imgur.com/260Qe2U.png)
This is the symptom

[Test File #2](https://github.com/jackiepiepkorn/cse15l-blog/blob/65caf524a5a2254b7675c08d014529b6a7b69dbe/my-test-file.md)

The bug is that the program thinks the image link is a link, which causes it to create the symptom of printing out the image link, even though it is not a link. The failure inducing input is the my-test-file.md, which has an image link, which is interpreted as a link by the program.

Here was my fix: ![Fixed Code](https://i.imgur.com/3MtAYKN.png)

</br>

## Code Change 3
![Image 3](https://i.imgur.com/ofBAnEV.png)
This is the symptom

[Test File #3](https://github.com/jackiepiepkorn/markdown-parser/blob/27134e270282d19265934716c26cf170f0536804/bracket-test.md)

The bug is that the program runs the loop infinitely after there are no more links, which causes it to create the symptom of the program running out of memory. The failure inducing input is the bracket-test.md, which has an extra bracket on the last line, which causes the while loop to infinitely run as it does not have a corresponding closing bracket.

Here was my fix: ![Fixed Code](https://i.imgur.com/HqP1ssf.png)





