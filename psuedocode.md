LL creation

head -> node1/pointer -> node2/pointer -> node4/pointer -> ... -> tail -> null

insertion - 3 cases

1. Insert at head
new_node -> next = head
all other pointers correct
2. Insert in middle
while (pointer !== position) {
    pointer = pointer -> next;
}
save store_next = pointer-> next
pointer -> next = new_node
new_node -> next = store_next

all other pointers correct
3. Insert at end
while (pointer -> next != null) {
    pointer = pointer -> next
}
pointer-> next = new_node
new_node -> next = null


