<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    Openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

## 743. Network Delay Time (Easy)

<p>
There are <code>N</code> network nodes, labelled <code>1</code> to <code>N</code>.
</p><p>
Given <code>times</code>, a list of travel times as <b>directed</b> edges <code>times[i] = (u, v, w)</code>, where <code>u</code> is the source node, <code>v</code> is the target node, and <code>w</code> is the time it takes for a signal to travel from source to target.
</p><p>
Now, we send a signal from a certain node <code>K</code>.  How long will it take for all nodes to receive the signal?  If it is impossible, return <code>-1</code>.
</p>

<p><b>Note:</b><br>
<ol>
<li><code>N</code> will be in the range <code>[1, 100]</code>.</li>
<li><code>K</code> will be in the range <code>[1, N]</code>.</li>
<li>The length of <code>times</code> will be in the range <code>[1, 6000]</code>.</li>
<li>All edges <code>times[i] = (u, v, w)</code> will have <code>1 <= u, v <= N</code> and <code>1 <= w <= 100</code>.</li>
</ol>
</p>

### Related Topics
  [[Heap](https://github.com/openset/leetcode/tree/master/tag/heap/README.md)]
  [[Depth-first Search](https://github.com/openset/leetcode/tree/master/tag/depth-first-search/README.md)]
  [[Breadth-first Search](https://github.com/openset/leetcode/tree/master/tag/breadth-first-search/README.md)]
  [[Graph](https://github.com/openset/leetcode/tree/master/tag/graph/README.md)]

### Hints
  1. We visit each node at some time, and if that time is better than the fastest time we've reached this node, we travel along outgoing edges in sorted order.  Alternatively, we could use Dijkstra's algorithm.