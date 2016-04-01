# Concurrent data structures #

This repository contains a recompilation of the available concurrent data structures on the web that support at least lock-free or wait-free properties. _If you know or own an implementation of a concurrent data structure, feel free to add it to the list_.

| Category | Name | Properties  | Language | Source |
| ----- |-----| -----|:-----:|-----|
| Stack      | Stack |lock-free |C |[Liblfds](http://liblfds.org/) |
| Stack      | Stack |lock-free |C++ |[Boost](http://www.boost.org/doc/libs/1_60_0/doc/html/lockfree.html) |
| Stack      | Stack | lock-free |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Stack      | Trieber Stack |  lock-free (based on Treiber's stack algorithm) |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_treiber_stack.html) |
| Stack      | FCStack |  lock-free, based on paper [2010] "Flat Combining and the Synchronization-Parallelism Tradeoff"|C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_f_c_stack.html) |
| Queue      | Queue |  |C |[Liblfds](http://liblfds.org/) |
| Queue      | Queue |  |C++ |[Boost](http://www.boost.org/doc/libs/1_60_0/doc/html/lockfree.html) |
| Queue      | Queue |  |Java |[Oracle](https://docs.oracle.com/javase/tutorial/essential/concurrency/collections.html) |
| Queue      | Queue |  |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Queue      | Deques |  |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Queue      | Bounded Queue |  |C |[Liblfds](http://liblfds.org/) |
| Queue      | Priority Queue |  |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Queue      | Priority Queue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_m_s_queue.html) |
| Queue      | Basket Queue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_basket_queue.html#details) |
| Queue      | MSQueue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_m_s_queue.html) |
| Queue      | RWQueue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_r_w_queue.html) |
| Queue      | MoirQueue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_moir_queue.html) |
| Queue      | Optimistic Queue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_optimistic_queue.html) |
| Queue      | Segmented Queue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_segmented_queue.html) |
| Queue      | FCQueue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_f_c_queue.html) |
| Queue      | Tsigas Cycle Queue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_tsigas_cycle_queue.html) |
| Queue      | Vyukov MPMC Cycle Queue |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_vyukov_m_p_m_c_cycle_queue.html) |
| Queue      | Ringbuffer (circular queue) |  |C |[Liblfds](http://liblfds.org/) |
| Queue      | Ringbuffer (circular queue) |  |C++ |[Boost](http://www.boost.org/doc/libs/1_60_0/doc/html/lockfree.html) |
| List      | LinkedList | lock-free  |C++ |[Lawrence Bush](http://people.csail.mit.edu/bushl2/rpi/project_web/page5.html) |
| List      | Free List |  |C |[Liblfds](http://liblfds.org/) |
| List      | Single LinkedList (ordered) |  |C |[Liblfds](http://liblfds.org/) |
| List      | Lazy List, Single LinkedList (ordered) |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_lazy_list.html) |
| List      | Michael List, Single LinkedList (ordered) |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_michael_list.html) |
| List      | Single LinkedList (unordered) |  |C |[Liblfds](http://liblfds.org/) |
| Map      | HashMap |  |C |[Liblfds](http://liblfds.org/) |
| Map      | Spllited Ordered List Map |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_split_list_map.html) |
| Map      | Stripped Map |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_striped_map.html) |
| Map      | Michael HashMap |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_michael_hash_map.html) |
| Map      | Skip List Map |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_skip_list_map.html) |
| Map      | Feldman Hashmap |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_feldman_hash_map.html) |
| Map      | HashMap |  |Java |[Oracle](https://docs.oracle.com/javase/tutorial/essential/concurrency/collections.html) |
| Map      | Map |  |Scala |[Root package](http://www.scala-lang.org/api/2.11.6/index.html#package) |
| Map      | Cuckoo Map |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_cuckoo_map.html) |
| Tree      | Binary Tree |  |C |[Liblfds](http://liblfds.org/) |
| Tree      | Ellen Binary Tree |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/namespacecds_1_1container_1_1ellen__bintree.html) |
| Tree      | Suffix Tree | Lookups are lock-free. Write operations are blocking  |Java |[Concurrent Suffix Trees](https://github.com/npgall/concurrent-trees) |
| Tree      | Radix Tree |Lookups are lock-free. Write operations are blocking  |Java |[Concurrent Suffix Trees](https://github.com/npgall/concurrent-trees) |
| Tree      | B Tree |  |C |[B-tree project](https://github.com/malbrain/Btree-source-code/) |
| Tree      | Red Black Tree |  |C |[University of Cambridge](http://www.cl.cam.ac.uk/research/srg/netos/projects/archive/lock-free/) |
| Tree      | AVL Tree |  |C++ |[Concurrent Trees project](https://github.com/wichtounet/btrees/) |
| Tree      | Bronson AVL Tree |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/namespacecds_1_1container_1_1bronson__avltree.html#details) |
| Tree      | Trie |  |Scala |[Root package](http://www.scala-lang.org/api/2.11.6/index.html#package) |
| Tree      | Heap |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/index.html) |
| Set      | Cuckoo Set |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_cuckoo_map.html) |
| Set      | Stripped Set |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_striped_set.html) |
| Set      | Feldman Hash Set |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_feldman_hash_set.html) |
| Set      | Skip List Set |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_skip_list_set.html) |
| Set      | Sets |  |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |


## Contributors ##

* Chien-Hao Chen
* Matías Bustos
* Joel Fuentes
