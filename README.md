# Data-structures-java
//deleting a node in a given postitioin
class GfG
{
    Node deleteNode(Node head, int x)
    {

	if(x==1)
	{
	    head=head.next;
	    return head;
	}
	else
	{
	    Node prev=null;
	    Node temp=head;
        for(int i=0;i<x-1;i++){
            prev=temp; 
	    temp=temp.next;
        }
        prev.next=temp.next;
	return head;
	
	}

    }
}
