# Tiny-ML
Tiny ML project for Embedded system/microcontroller 
So, consider if I give you a set of numbers like this:

X: -1, 0, 1, 2, 3, 4

And then I give you another set of numbers like this:

Y: -3, -1, 1, 3, 5, 7

Can you figure out the relationship between the two sets? There’s a function that converts -1 to -3, 0 to -1, 1 to 1, 2 to 3, 3 to 5 and 4 to 7. Can you figure out the relationship. Think about it for a moment.

Often when I ask people about it, they see that the 0 is matched to -1, so Y is (something) times X - 1. Maybe they’ll take a guess at the something, and come up with 3.

Then fill in the gaps, if Y=3X-1, then

X: -1, 0, 1, 2, 3, 4

Becomes

Y: -4, -1, 2, 5, 8, 11

Other than working for 0, it fails for everything else. In ML terms, you can define this as your loss is ‘high’.  With what you learned from that, you might think, what if it’s Y=2X-1?

Then, when you fill in the results for Y=2X-1, you’ll get:

X: -1, 0, 1, 2, 3, 4

Becomes

Y: -3, -1, 1, 3, 5, 7

...which matches your original data perfectly. Your loss is zero.

You’ve just gone through this process:
