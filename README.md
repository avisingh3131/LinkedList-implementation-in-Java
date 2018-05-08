// LinkedList-implementation-in-Java
//Single LinkedList implementation

class Node{
  int data;
  Node next;
}
 class LinkedList{
    Node head=null;
 //to insert a new value from the tail.
    void insert(int data){
      Node node=new Node();
       node.data=data;
       node.next=null;
      if(head==null){
       head=node;
       }
     else{
     Node n=head;
     while(n.next!=null){
        n=n.next;
       }n.next=node;
     }
 }
 //to print the data by traversing the LinkedList
  void print(){
        Node temp=head;
       while(temp!=null){
     System.out.print(temp.data);
     System.out.print(" ");
      temp=temp.next;
         }
     }
  }
 public class MyClass{
   public static void main(String[] args){
    LinkedList l=new LinkedList();
    l.insert(1);
    l.insert(2);
    l.insert(3);
     l.insert(4);
     l.insert(5);
     l.print();
   }
 }
 
//o/p;- 1 2 3 4 5  
