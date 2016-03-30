# Concurrent data structures #

The following repository contains a recompilation of the available concurrent data structures on the web that support at least lock-free or wait-free properties.

| Category | Name | Properties  | Language | Source |
| ----- |-----| -----|:-----:|-----|
| Stack      | Stack |  |C |[Liblfds](http://liblfds.org/) |
| Stack      | Stack |  |C++ |[Boost](http://www.boost.org/doc/libs/1_60_0/doc/html/lockfree.html) |
| Stack      | Stack |  |Ada |[NBAda](http://www.gidenstam.org/Ada/Non-Blocking/) |
| Stack      | Trieber Stack |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_treiber_stack.html) |
| Stack      | FCStack |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_f_c_stack.html) |
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
| List      | LinkedList |  |C++ |[Lawrence Bush](http://people.csail.mit.edu/bushl2/rpi/project_web/page5.html) |
| List      | Free List |  |C |[Liblfds](http://liblfds.org/) |
| List      | Single LinkedList (ordered) |  |C |[Liblfds](http://liblfds.org/) |
| List      | Lazy List, Single LinkedList (ordered) |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_lazy_list.html) |
| List      | Michael List, Single LinkedList (ordered) |  |C++ |[cds](http://libcds.sourceforge.net/doc/cds-api/classcds_1_1container_1_1_michael_list.html) |
| List      | Single LinkedList (unordered) |  |C |[Liblfds](http://liblfds.org/) |
| Map      | HashMap |  |C |[Liblfds](http://liblfds.org/) |


## Contributors ##

* Chien-Hao Chen
* Matías Bustos
* Joel Fuentes
