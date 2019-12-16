# iebis_swdev_exam_debugging

I noticed that the YFT Upper size letters where not printing in the console, from this I infered something was wrong.

##Bug 1
The correct format for adding a new StringBuffer value is not: 
word = new StringBuffer('Y');
it is 
word = new StringBuffer("Y");

Bug found here: https://www.geeksforgeeks.org/stringbuffer-class-in-java/
## Bug2
Now that I ran the code multiple times, I spotted that only the "Tour" would print
I thought something was wrong with the random.nextInt but when printing that, it was working fine so I looked into
how switch statements work and it turns out that they need a break. 
Found this here: https://stackoverflow.com/questions/37383521/switch-statement-in-generating-random-numbers-in-java-not-working

When I added the break, The code was printing Your and Tour and Four 