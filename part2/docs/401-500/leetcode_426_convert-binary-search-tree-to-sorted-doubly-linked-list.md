# $426. [中等] 将二叉搜索树转化为排序的双向链表

**题目链接：**[https://leetcode-cn.com/problems/convert-binary-search-tree-to-sorted-doubly-linked-list](https://leetcode-cn.com/problems/convert-binary-search-tree-to-sorted-doubly-linked-list)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>将一个二叉搜索树就地转化为一个已排序的双向循环链表。可以将左右孩子指针作为双向循环链表的前驱和后继指针。</p> 
  <p>为了让您更好地理解问题，以下面的二叉搜索树为例：</p> 
  <p>&nbsp;</p> 
  <p><img style="width: 250px;" src="/uploads/2018/10/12/bstdlloriginalbst.png"></p> 
  <p>&nbsp;</p> 
  <p>我们希望将这个二叉搜索树转化为双向循环链表。链表中的每个节点都有一个前驱和后继指针。对于双向循环链表，第一个节点的前驱是最后一个节点，最后一个节点的后继是第一个节点。</p> 
  <p>下图展示了上面的二叉搜索树转化成的链表。“head” 表示指向链表中有最小元素的节点。</p> 
  <p>&nbsp;</p> 
  <p><img style="width: 400px;" src="/uploads/2018/10/12/bstdllreturndll.png"></p> 
  <p>&nbsp;</p> 
  <p>特别地，我们希望可以就地完成转换操作。当转化完成以后，树中节点的左指针需要指向前驱，树中节点的右指针需要指向后继。还需要返回链表中的第一个节点的指针。</p> 
  <p>下图显示了转化后的二叉搜索树，实线表示后继关系，虚线表示前驱关系。</p> 
  <p>&nbsp;</p> 
  <p><img style="width: 400px;" src="/uploads/2018/10/12/bstdllreturnbst.png"></p> 
 </div>
</div>

---

```java
/*
// Definition for a Node.
class Node {
    public int val;
    public Node left;
    public Node right;

    public Node() {}

    public Node(int _val) {
        val = _val;
    }

    public Node(int _val,Node _left,Node _right) {
        val = _val;
        left = _left;
        right = _right;
    }
};
*/
class Solution {
    public Node treeToDoublyList(Node root) {
        
    }
}
```