# RBTree 개요

## Red-Black Tree란?

- 레드-블랙 트리(red-black tree)는 자가 균형 이진 탐색 트리(self-balancing binary search tree)로서, 대표적으로는 연관 배열 등을 구현하는 데 쓰이는 자료구조다.
- 레드-블랙 트리는 복잡한 자료구조지만, 실 사용에서 효율적이고, 최악의 경우에도 상당히 우수한 실행 시간을 보인다: 트리에 n개의 원소가 있을 때 O(log n)의 시간복잡도로 삽입, 삭제, 검색을 할 수 있다.

## RBTree 특성 (5개)

- `#1`. 모든노드 RED / BLACK
- `#2`. **루트노드는 BLACK**
- `#3`. 모든 NIL 노드는 BLACK
- `#4`. 노드가 RED 면, 자녀는 BLACK (**RED는 연속하면 안됨**)
- `#5`. 임의의 경로(자신을 제외)부터 **자손 NIL 까지 BLACK 개수는 동일**

## RB 트리는 어떻게 균형을 잡는가?

<aside>
💡 삽입/삭제시 `#2, #4, #5` 속성을 위반함. 이들을 해결하기 위해서 구조를 바꾸면, 자연스럽게 균형이 잡히게 된다.

</aside>

## 참조
https://en.wikipedia.org/wiki/Red%E2%80%93black_tree
