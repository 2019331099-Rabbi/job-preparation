
# Solutions
**Part 1: Coding**
1. The worst case of Quicksort occurs when the array is already sorted.
2. The prerequisite of binary search is that the array must be sorted.
3. The best time complexity of merge sort is O(nlogn) and worst time complexity is O(n^2)
4. Minimal Spanning tree does not give the shortest distance between any 2 specified nodes.
5. log q (base p) = log q (base k) / log p (base k)
6. a = b, b = a/2
  
7.
```
bool myFun(int N) { return (N & (N-1)) == 0;}
```

8.
```
 int secMin(int nums[], int len) {
  int cnt[100005], i, j, val, mn = INT_MAX;
  memset(cnt, 0, sizeof(cnt));
  for (i = 0; i < len; i++) {
      val = nums[i];
      cnt[val] += 1;
      if (val < mn) {
          mn = val;
      }
  }
  if (cnt[mn] > 1) {
      return mn;
  }

  for (i = mn+1; i <= 100000; i++) {
      if (cnt[i] > 0)
          return i;
  }
}
```

