you got an image
every pixel is mapped between 0 and 255
you apply [[Binarization]] to it.

your image with some noise around the object you want.

pass them by a global threshold parameter to get a better image
or
you can do a local filtering, a local threshold

now you have a single connected component character.

this is the first step for OCR
now, draw and outline around it.


you have now just an image,
you don't know the font.
you don't know what type of character it is in what kind of language.
Larry Spitz was able to identify what language is just by the character set of the components.


classification
by the alphabet


pattern matching
brutal, I don't have the right font, I might not have a good match.





training sets, Deep learning, Artificial Intelligence.




