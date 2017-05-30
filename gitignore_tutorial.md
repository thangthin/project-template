Globbing Crash Course
Let's say that you add 50 images to your project, but want Git to ignore all of them. Does this mean you have to list each and every filename in the .gitignore file? Oh gosh no, that would be crazy! Instead, you can use a concept called globbing.

Globbing lets you use special characters to match patterns/characters. In the .gitignore file, you can use the following:

```
blank lines can be used for spacing
# - marks line as a comment
* - matches 0 or more characters
? - matches 1 character
[abc] - matches a, b, or c
** - matches nested directories - a/**/z matches
a/z
a/b/z
a/b/c/z
So if all of the 50 images are JPEG images in the "samples" folder, we could add the following line to .gitignore to have Git ignore all 50 images.
```
```
samples/*.jpg
```