# Lab Report 4

### [Link to My Markdown Parse Repository](https://github.com/jackiepiepkorn/markdown-parser)
### [Link to the Repository We Reviewed](https://github.com/ryankosta/good-markdown-parser)

## Snippet 1

### Test for Snippet 1:
![Test for Snippet 1](https://i.imgur.com/ibm6K0f.png?1)
It should produce only 'another link' as a link, which I saw on commonmark.org

### Output of the test on my repo:
![Test Fail Snippet 1](https://i.imgur.com/FM0mLIc.png?1)
There is a failure.

### Output of the test on their repo:
![Test Fail Snippet 1](https://i.imgur.com/gved9u8.png?1)
There is a failure.

### How I Can Change My Code
I can try to make sure the link is not outputted if there is a backtick without a pair. Only the links with pairs, not backticks without a pair, will be outputted.

## Snippet 2

### Test for Snippet 2:
![Test for Snippet 2](https://i.imgur.com/tmib6zg.png?1)
It should produce all links except the b.com one.

### Output of the test on my repo:
![Test Fail Snippet 2](https://i.imgur.com/ncZ2rEK.png?1)
There is a failure.

### Output of the test on their repo:
![Test Fail Snippet 2](https://i.imgur.com/5ONAVKO.png?1)
There is a failure.

### How I Can Change My Code
I can make sure that links with a opening parenthesis without a corresponding closing one will not be outputted.

## Snippet 3

### Test for Snippet 3:
![Test for Snippet 3](https://i.imgur.com/1CBpWvG.png?1)
It should produce only the link for the CSE schedule.

### Output of the test on my repo:
![Test Fail Snippet 3](https://i.imgur.com/ZfSLuMk.png?1)
There is a failure.

### Output of the test on their repo:
![Test Fail Snippet 3](https://i.imgur.com/jpAd1TP.png?1)
There is a failure.

### How I Can Change My Code
Because the issue was caused by linebreaks and extra spaces, I can code my MarkdownParse to make sure that it does not count linebreaks or large gaps in its parsing.
