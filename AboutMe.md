# Shaik

i'm doing my masters in Northwest Missouri State university.
i want to see myself as a Software Developer.
That's me.

![myImage](images/Shaik_pp.jpg)

------

table

------

This table is all about sport or activity and three columns consists of name of the sport, location, amount of money

| sport/activity | Location | Amount |
|---|---|---|
|Cricket | England | 300|
|Hockey | India | 200|
|Football | France | 400|
| Basketball | Serbia | 700|

-----
Quotes i like 

------------

>stay hungry stay foolish

*steve jobs*

>Sometimes life hits you in the head with a brick. Don't lose faith.

*steve jobs*

--------
code fencing
--------

>In computational geometry, a sweep line algorithm or plane sweep algorithm is an algorithmic paradigm that uses a conceptual sweep line or sweep surface to solve various problems in Euclidean space. It is one of the key techniques in computational geometry.

REFERENCE TO THE ABOVE SUMMARY<https://en.wikipedia.org/wiki/Sweep_line_algorithm>

```
int[] res = new int[intervals.length];
 Arrays.fill(res, -1);
 
 List<Point> points = new ArrayList<>();
 for (int i = 0; i < intervals.length; i++) {
     points.add(new Point(intervals[i].start, 1, i));
     points.add(new Point(intervals[i].end, 0, i));
 }
 
 Collections.sort(points);
 
 List<Integer> prevIdxs = new ArrayList<>();
 
 for (Point point: points) {
     if (point.flag == 1) {
             for (Integer prevIdx: prevIdxs) {
                res[prevIdx] = point.index; 
             }
             prevIdxs = new ArrayList<>();
     } else {
         prevIdxs.add(point.index);
     }
 }
 
 return res
 ```

 REFERENCE TO THE ABOVE CODE<https://leetcode.com/problems/find-right-interval/discuss/91797/java-sweep-line-solution-onlogn>






