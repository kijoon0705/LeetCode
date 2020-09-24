# 175. Combine Two Tables
> QUESTION: Write a SQL query for a report that provides the following information for each person in the Person table, regardless if there is an address for each of those people:

***

#### [QUIZ] 
+ LeetCode: [detailed explanation](https://leetcode.com/problems/combine-two-tables/, "detailed explanation")

#### [Sudo]
+ 'combine'이라는 단어에서 테이블 Join 문제라는것을 파악.
+ Join 중 어떤 Join을 정해야할지 생각하는게 포인트였다. 

#### [Code]
<code>
<pre>
SELECT FirstName, LastName, City, State
FROM person
LEFT JOIN address on person.personid = address.personid
</code>
</pre>
