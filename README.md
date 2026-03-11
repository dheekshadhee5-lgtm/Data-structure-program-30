# Data-structure-program-30
#include <stdio.h>
#include <stdlib.h>
Struct node{
 Int data;
 Struct node *left,*right;
};
Struct node* newNode(int 
data){
 Struct node* temp=(struct 
node*)malloc(sizeof(struct 
node));
 Temp->data=data;
 Temp->left=temp-
>right=NULL;
 Return temp;
}
Struct node* insert(struct 
node* root,int data){
 If(root==NULL) return 
newNode(data);
 If(data < root->data)
 Root->left=insert(root-
>left,data);
 Else
 Root->right=insert(root-
>right,data);
 Return root;
>Void inorder(struct node* 
root){
 If(root){
 Inorder(root->left);
 Printf(“%d “,root->data);
 Inorder(root->right);
 }
}
Int main(){
 Struct node* root=NULL;
 Root=insert(root,50);
 Root=insert(root,30);
 Root=insert(root,70);
 Printf(“Library Book 
IDs:\n”);
 Inorder(root);
 Return 0;
}
OUTPUT 
Library Book IDs:
30 50 70
