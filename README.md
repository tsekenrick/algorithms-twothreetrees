There will be a single type of query to the database

* given two planet names return the list of planet names and entrance fees of all planets between the two queried names, in lexicographic order

### Input Format

The first line contains a number *n*, which is the size of the database.

The next *n* lines are of the form
* *a k*

*a* - the planet name, *k* - the entrance fee of the planet, separated by a single space.

The next line contains a number  the number of queries to the database.

The next *m* lines are of the form
* *a b*

*a b* - planet names.

### Constraints
*n, m <= 1000*
*|a|, |b| <= 10*
*0 <= k <= 10^9*

YOU MUST USE 2-3 TREE DATA STRUCTURES PROVIDED IN CLASS

To avoid time-outs, each range query *a b* should run in time *O(logn)* plus the number of planets in the range *a...b*

### Output Format

For each query write down the names of the planets and the entrance fees, separated by a single space, in between (inclusive) *a,b*, in separate lines.

### Sample Input 0

```
3
earth 10
venus 30
jupiter 5
2
earth jupiter
earth venus
```

### Sample Output 0

```
earth 10
jupiter 5
earth 10
jupiter 5
venus 30
```

### Sample Input 1

```
3
earth 10
venus 30
jupiter 5
2
a z
venus earth
```

### Sample Output 1

```
earth 10
jupiter 5
venus 30
earth 10
jupiter 5
venus 30
```
