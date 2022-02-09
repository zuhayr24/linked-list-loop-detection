# linked-list-loop-detection
Node *s=head;
    Node *f=head;
    while(f!=NULL && f->next!=NULL)
    {
        s=s->next;
        f=f->next->next;
        if(s==f)
        {
            return 1;
        }
    }
    return 0;
