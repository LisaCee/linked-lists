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

deletion - 3 cases

1. Delete head
pointer to head, delete link/delete data(memory)
pointer to next_node (new head)
return new head

node* delete(node*head, char d) {
    q = head
    p = head -> next
    if (q -> data == d) {
        head = p;
        delete(q)
    }
    else {
        while (p -> data != d) {
            p = n -> next;
            q = q -> next;
        }
        if (p -> next == null) {
            last node
            q -> next = null;
            delete(p)
        } else {
            internal node
            q - > next = p -> next;
            delete(p)
        }
    } return head node from new
}

2. Delete internal node (not head/tail)
pointer of previous -> next's pointer location

3. Delete tail
Make second to last node point to null
delete data(memory)