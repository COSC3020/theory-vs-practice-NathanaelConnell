# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

1. reason number one that asymptotic analusis could be misleading compared to actual performance is that it doenst always take into acount the size of the data that is being worked with
2. reason number two is the actual implementation of the algortihm could be very bad even if its fast asymptotically it could be a slow implementation of the algorithm
3. reason number 3 is the hardware that is being used varies a lot and a very quick asymptotic algorithm could be a lot slower or faster depending on what hardware it is being run on.

I would guess that it takes 50 seconds in a generic case because if it is just a O(n) type of analysis then it should move up linearly and if there is 1000 to 10000 then the time should move up by ten times giving 5 to 50 seconds

1. reason number 1 it might take 100 secodns is that the asymptotic complexity is higher than linear and might go up exponentially with larger data sets
2. reason number 2 is that 10000 might be to big of a data set for the specific hardware or machine making it slow down due to memory constraints
3. reason number 3 is that there might be a part of the algorithm that is constructed poorly for when handeling larger sizes of data sets that it can run quicker with smaller data sets on.

"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice."
