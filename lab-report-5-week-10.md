# Lab Report 5

## How I found the tests with different results:

My group used vimdiff on the results of running a bash for loop.

## Two test files with different results:

[14.md](https://github.com/nidhidhamnani/markdown-parser/blob/8dd87e6914ae40a4321aac8e2483e349de40b03c/test-files/14.md) & 
[194.md](https://github.com/nidhidhamnani/markdown-parser/blob/8dd87e6914ae40a4321aac8e2483e349de40b03c/test-files/194.md)

## Test 1 (14.md)
Here are the actual outputs:
![Actual outputs](https://i.imgur.com/AbPTDBo.png?1)
The link output shouldn't have been any links, so only our code was correct in its output.
### Bug fix:
In order to fix the provided MarkdownParser, we would need to fix the part where it detects an open bracket. We want it to not output any links that have a backslash in them, as a link cannot contain a backslash and people typically put backslashes in links to avoid it becoming a hyperlink. This is the area of code I would edit:
![Editing for #14](https://i.imgur.com/q9MszYW.png?1)

## Test 2 (194.md)
Here are the actual outputs:
![Actual outputs](https://i.imgur.com/ZlO8E09.png?1)
The link output should have been "Foo*bar]", so both markdown parse codes were wrong in their outputs.
### Bug fix:
If we focus on fixing the provided Markdown Parser code, we can change the code to consider that there might be extra characters between the link name and the link itself. This is the area of code I would edit:
![Editing for #194](https://i.imgur.com/NwhDlOg.png?1)
