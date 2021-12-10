1. Serial program


* Compile : gcc -g -Wall -o serial_linked_list serial_linked_list.c
* Run : ./serial_linked_list <n> <m> <mMember> <mInsert> <mDelete>
   * n - number of nodes in the linked list
   * m - number of random operations
   * mMember - fraction of member operations
   * mInsert - fraction of insert operations
   * mDelete - fraction of delete operations


2. Parallel program (based on Pthreads) with one mutex for the entire linked list


* Compile : gcc -g -Wall -o mutex_linked_list mutex.c -lpthread
* Run : ./mutex_linked_list <n> <m> <mThreadCount><mMember> <mInsert> <mDelete>


3. Parallel program (based on Pthreads) with read-write locks for the entire linked list


* Compile : gcc -g -Wall -o rwlock_linked_list rwlock.c -lpthread
* Run : ./mutex_linked_list <n> <m> <mThreadCount> <mMember> <mInsert> <mDelete>