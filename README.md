Pool-object_pool
================

boost object_pool in Pool namespace with free(ptr) O(1) instead of O(n)

(actually O(lg n) amortized; free list is sorted on ~object_pool, but only if you freed
individual items)

see https://github.com/graehl/boost/tree/object_pool-constant-time-free for a version
that overwrites the (unmaintained) boost::object_pool
