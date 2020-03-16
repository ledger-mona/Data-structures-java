# Data-structures-java
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
	    Node n1=null;
	    Node n=head;
	    for(int i=1;i<x-1;i++)
	    {
	        n=n.next;
	    }
	    n1=n.next;
	    n.next=n1.next;
	    n1=null;
	    return head;
	
	}

    }
}
