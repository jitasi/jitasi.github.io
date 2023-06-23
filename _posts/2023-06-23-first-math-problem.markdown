---
layout: post
title:  "The First Math Problem"
date:   2023-06-23 00:17:46 -0700
categories: math counting
tags: tag-math tag-counting
comments: "true"
inlinecomments: "true"
mathjax: "true"
---
(Lehigh MC-2018-19) How many 6-digit numbers whose leftmost digit is 1 have exactly two pairs of identical digits (and no digit occurs three or more times)?

Note 1: Casework is often an effective approach for solving a wide range of counting problems that involve digits or numbers.

Solution: 

Regardless of the order of this 6 digit, we have the numbers in the format like AABBCD. Since 1 must be choose, we can do casework by if 1 is A/B or C/D. 

case 1: 1 is A/B. We need to choose one digit for A/B and two digits for C/D. There are a total of 9 choices for the A/B digit, and we can select 2 digits from the remaining 8 digits for C/D, yielding a count of $9 \times {8 \choose 2}$.

case 2: 1 is C/D. we need to choose one digit for C/D and two digits for A/B. Again, there are 9 choices for the C/D digit, and we can select 2 digits from the remaining 8 digits for A/B, resulting in a count of $9 \times {8 \choose 2}$.

Now, let's consider the order of the six digits.

case 1: When 1 is in the leftmost position, we can choose another position for the second 1, which has 5 possibilities. Next, we select 2 positions for another pair of identical digits, which can be done in $4 \choose 2$ ways, Lastly, we have 2 choices for the remaining C/D digit. Thus, there are $5 \times {4 \choose 2} \times 2$ possibilities in this case.

case 2: When 1 is in the leftmost position, we choose another position for the C/D digit, which has 5 possibilities. Then, we arrange the A/B digits, which can be done in ${4 \choose 2}$ ways since they are identical. Thus, there are ${4 \choose 2} \times 5$ possibilities in this case.

Combining both cases, the total count is:
${9 \times {8 \choose 2} \times {5 \times {4 \choose 2} \times 2}}  +  9 \times {8 \choose 2} \times {4 \choose 2} \times 5 = 22680$.