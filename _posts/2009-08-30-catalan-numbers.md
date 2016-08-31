---
layout: post
title:  "Catalan Numbers"
date:   2009-08-30 12:00:00
categories: ['blog']
bigimg: '/img/catalan_numbers.png'
---
Recently I was trying to count the number of n-bit numbers that have an equal number of 1’s and 0’s.  For example, there are 6 such numbers for 4-bit long numbers (0011, 0101, 0110, 1001, 1010, 1100).  I wrote a simple program to count such numbers for arbitrarily long numbers.  However, the program was computationally complex and it took a long time to compute the result for large values of n.  After spending some time trying to figure out the equation myself, I searched the internet and stumbled upon Catalan numbers.  I determined that the equation is related to Catalan numbers.  I included the equation below because I couldn’t find it anywhere else.  Also, I don’t have a formal proof, but it seems to work.  Enjoy!

Number of n-bit numbers that have an equal number of 1’s and 0’s = (m+1) * Cm, where m = n/2 and Cm = mth Catalan number
