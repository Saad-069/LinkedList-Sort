# LinkedList-Sort
void sort() {
	int tem1, tem2;
	tem2 = noofnodes();
	Node* temp;
	for (int i = 0; i < tem2; i++) {

		temp = head;
		while (temp->next != NULL) {

			if (temp->data > temp->next->data) {
				tem1=temp->data;
				temp->data = temp->next->data;
				temp->next->data = tem1;
			}



			temp = temp->next;
		}

	}
	
	
}
