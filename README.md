# Concurrent data structures #

This repository contains a compilation of the available concurrent data structures on the web that support at least lock-free or wait-free properties. Some lock-based fine-grained synchronization approaches, that are competitive with lock-free approaches, are also considered. _If you know or own an implementation of a concurrent data structure, feel free to add it to the list_.

| Category | Name | Properties  | Language | Source |
| ----- |-----| -----|:-----:|-----|
| Stack      | Stack |lock-free |C |[Liblfds](http://liblfds.org/) |
| Stack      | Stack |lock-free |C++ |[Boost](http://www.boost.org/doc/libs/1_60_0/doc/html/lockfree.html) |
| Stack      | Stack | lock-free |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Stack      | Trieber Stack |  lock-free (based on Treiber's stack algorithm) |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_treiber_stack.html) |
| Stack      | FCStack |  lock-free, based on paper [2010] "Flat Combining and the Synchronization-Parallelism Tradeoff"|C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_f_c_stack.html) |
| Queue      | Queue | lock-free |C |[Liblfds](http://liblfds.org/) |
| Queue      | Queue | lock-free multi-produced/multi-consumer queue |C++ |[Boost](http://www.boost.org/doc/libs/1_60_0/doc/html/lockfree.html) |
| Queue      | Queue | lock-free queue of bounded and dynamic size |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Queue      | Deques | lock-free deques of dynamic size |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Queue      | Bounded Queue | lock-free |C |[Liblfds](http://liblfds.org/) |
| Queue      | Priority Queue | lock-free priority queues of dynamic size |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Queue      | Basket Queue | basket lock-free queue (non-intrusive variant)  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_basket_queue.html#details) |
| Queue      | MSQueue | Michael & Scott lock-free queue |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_m_s_queue.html) |
| Queue      | RWQueue | Michael & Scott blocking queue with fine-grained synchronization schema |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_r_w_queue.html) |
| Queue      | MoirQueue | variation of Michael & Scott's lock-free queue |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_moir_queue.html) |
| Queue      | Optimistic Queue | lock-free, based on paper [2008] Edya Ladan-Mozes, Nir Shavit "An Optimistic Approach to Lock-Free FIFO Queues"  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_optimistic_queue.html) |
| Queue      | Segmented Queue | based on paper [2010] Afek, Korland, Yanovsky "Quasi-Linearizability: relaxed consistency for improved concurrency" |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_segmented_queue.html) |
| Queue      | FCQueue | Flat combining queue based on paper by Hendler, Incze, Shavit and Tzafrir [2010] "Flat Combining and the Synchronization-Parallelism Tradeoff" |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_f_c_queue.html) |
| Queue      | Tsigas Cycle Queue | non-intrusive implementation of Tsigas & Zhang cyclic queue based  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_tsigas_cycle_queue.html) |
| Queue      | Vyukov MPMC Cycle Queue | multi-producer multi-consumer (MPMC), array-based, fails on overflow, does not require GC, w/o priorities, causal FIFO, blocking producers and consumers queue. The algorithm is pretty simple and fast. It's not lock-free in the official meaning, just implemented by means of atomic RMW operations w/o mutexes. |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_vyukov_m_p_m_c_cycle_queue.html) |
| Queue      | Ringbuffer (circular queue) | lock-free |C |[Liblfds](http://liblfds.org/) |
| Queue      | Ringbuffer (circular queue) |  lock-free multi-produced/multi-consumer queue |C++ |[Boost](http://www.boost.org/doc/libs/1_60_0/doc/html/lockfree.html) |
| List      | LinkedList | lock-free  |C++ |[Lawrence Bush](http://people.csail.mit.edu/bushl2/rpi/project_web/page5.html) |
| List      | Free List | lock-free |C |[Liblfds](http://liblfds.org/) |
| List      | Single LinkedList (ordered) | lock-free |C |[Liblfds](http://liblfds.org/) |
| List      | Lazy List, Single LinkedList (ordered) | based on an optimistic locking scheme for inserts and removes, eliminating the need to use the equivalent of an atomically markable reference. Based on paper [2005] Steve Heller, Maurice Herlihy, Victor Luchangco, Mark Moir, William N. Scherer III, and Nir Shavit "A Lazy Concurrent List-Based Set Algorithm"  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_lazy_list.html) |
| List      | Michael List, Single LinkedList (ordered) | based on paper [2002] Maged Michael "High performance dynamic lock-free hash tables and list-based sets" |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_michael_list.html) |
| List      | Single LinkedList (unordered) | lock-free |C |[Liblfds](http://liblfds.org/) |
| Map      | HashMap | lock-free |C |[Liblfds](http://liblfds.org/) |
| Map      | Spllited Ordered List Map |  based on split-ordered list algorithm discovered by Ori Shalev and Nir Shavit, see [2003] Ori Shalev, Nir Shavit "Split-Ordered Lists - Lock-free Resizable Hash Tables" and [2008] Nir Shavit "The Art of Multiprocessor Programming" |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_split_list_map.html) |
| Map      | Stripped Map | striped hash map based on lock striping technique by [2008] Maurice Herlihy, Nir Shavit "The Art of Multiprocessor Programming"  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_striped_map.html) |
| Map      | Michael HashMap | based on lock'free ordered list by [2002] Maged Michael "High performance dynamic lock-free hash tables and list-based sets" |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_michael_hash_map.html) |
| Map      | Skip List Map | lock-free variant of skip-list implemented according to book [2008] M.Herlihy, N.Shavit "The Art of Multiprocessor Programming", chapter 14.4 "A Lock-Free Concurrent Skiplist" |C++|[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_skip_list_map.html) |
| Map      | Feldman Hashmap | hash map based on multi-level array. Based on paper [2013] Steven Feldman, Pierre LaBorde, Damian Dechev "Concurrent Multi-level Arrays: Wait-free Extensible Hash Maps" |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_feldman_hash_map.html) |
| Map      | HashMap |  |Java |[Oracle](https://docs.oracle.com/javase/tutorial/essential/concurrency/collections.html) |
| Map      | Map |  |Scala |[Root package](http://www.scala-lang.org/api/2.11.6/index.html#package) |
| Map      | Cuckoo Map |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_cuckoo_map.html) |
| Map      | Fast Concurrent Memoization Map | Fast Concurrent Memoization Map (fcmm) is an almost lock-free concurrent hashmap written in C++11 to be used for memoization in concurrent environments. | C++ | [fcmm](https://github.com/giacomodrago/fcmm) |
| Map      | Junction | Junction is a library of concurrent data structures in C++. It contains several hash map implementations. | C++ | [junction](https://github.com/preshing/junction) |
| Tree      | Binary Tree | lock-free |C |[Liblfds](http://liblfds.org/) |
| Tree | Binary Tree | non-blocking BST (external) | | [paper (2010)] (http://dl.acm.org/citation.cfm?id=1835736)| 
| Tree      | Ellen's Binary Tree |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/namespacecds_1_1container_1_1ellen__bintree.html) |
| Tree | Natarajan's Binary Search Tree | lock-free BST (external) | | [paper (2014)](http://dl.acm.org/citation.cfm?id=2555256)| 
| Tree | Howley's Binary Search Tree | non-blocking internal BST | | [paper (2012)](http://dl.acm.org/citation.cfm?id=2312036) |
| Tree | Ramachandran's Binary Search Tree | lock-free internal BST | | [paper (2015)](http://dl.acm.org/citation.cfm?id=2684472) |
| Tree      | Suffix Tree | Lookups are lock-free. Write operations are blocking  |Java |[Concurrent Suffix Trees](https://github.com/npgall/concurrent-trees) |
| Tree      | Radix Tree |Lookups are lock-free. Write operations are blocking  |Java |[Concurrent Suffix Trees](https://github.com/npgall/concurrent-trees) |
| Tree      | B Tree |  |C |[B-tree project](https://github.com/malbrain/Btree-source-code/) |
| Tree      | Red Black Tree |  |C |[University of Cambridge](http://www.cl.cam.ac.uk/research/srg/netos/projects/archive/lock-free/) |
| Tree | Red Black Tree | Wait-free red black tree | | [paper](https://pdfs.semanticscholar.org/5afc/38731711a6516640e360c8f8394707bbff19.pdf) |
| Tree      | Bronson AVL Tree |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/namespacecds_1_1container_1_1bronson__avltree.html#details) |
| Tree      | Trie |  |Scala |[Root package](http://www.scala-lang.org/api/2.11.6/index.html#package) |
| Tree      | Heap |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/index.html) |
| Set      | Cuckoo Set | Cuckoo hash map based on papers [2007] M.Herlihy, N.Shavit, M.Tzafrir "Concurrent Cuckoo Hashing. Technical report" and [2008] Maurice Herlihy, Nir Shavit "The Art of Multiprocessor Programming"  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_cuckoo_map.html) |
| Set      | Stripped Set | Striped hash set based on approach proposed in [2008] Maurice Herlihy, Nir Shavit "The Art of Multiprocessor Programming"  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_striped_set.html) |
| Set      | Feldman Hash Set | hash set based on multi-level array. Based on approached proposed in [2013] Steven Feldman, Pierre LaBorde, Damian Dechev "Concurrent Multi-level Arrays: Wait-free Extensible Hash Maps"  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_feldman_hash_set.html) |
| Set      | Skip List Set | lock-free variant of skip-list implemented according to book [2008] M.Herlihy, N.Shavit "The Art of Multiprocessor Programming", chapter 14.4 "A Lock-Free Concurrent Skiplist"  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_skip_list_set.html) |
| Set      | Sets | lock-free sets of dynamic size |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Ring Buffer      | Ring Buffer | Lock-free multi-producer single-consumer (MPSC) ring buffer | C++ |[rmind/ringbuf](https://github.com/rmind/ringbuf) |
| Container library      | Tervel | Wait-free | C++ |[Tervel](https://ucf-cs.github.io/Tervel/index.html) |


## Contributors ##

* Joel Fuentes
* Chien-Hao Chen
* Matías Bustos
* Simon Giesecke
