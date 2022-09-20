/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     ListNode *next;
 *     ListNode() : val(0), next(nullptr) {}
 *     ListNode(int x) : val(x), next(nullptr) {}
 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
 * };
 */
class Solution {
public:
    ListNode* deleteDuplicates(ListNode* head) {
        if(head==NULL){return head;}
        ListNode* ptr=head->next;
        ListNode* curr=head;
        ListNode* ret=curr;
        while(ptr!=NULL){
            if(curr->val!=ptr->val){
                curr->next=ptr;
                curr=curr->next;
            }
            ptr=ptr->next;
        }
        curr->next=ptr;
        return ret;
    }
};
