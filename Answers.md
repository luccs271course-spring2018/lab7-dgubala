#Lab5 Questions
Q:Why does LinkedStack not require an explicit constructor?

A:LinkedStack does not need an explicit constructor because it uses the implementation iStack

Q:What is the time and (extra) space complexity of each of the LinkedStack methods, as well as ReverseLines.main?

A:
LinkedStack:
    push = O(1)
    isEmpty = O(1)
    peek= O(n)
    pop= O(n)
    asList= O(n)

ReverseLines: O(n)
    

Q:How else (not using Node) could we have implemented LinkedStack in such a way that it is still based on a linked list but the asList method uses constant time and space?

A; Use a LinkedList 
    public ListStack() { 
        list = new LinkedList<>(); 
    }

Q:Is it better for push and pop to return the item or the stack itself? Briefly discuss the pros and cons of each design.

A:return stack
    pros: All items are visible
    cons: takes more time
  
  return the item
    pros:takes less time, you can reveive the items individually
    cons: Other items in the stack are not visible, it only returns one single item