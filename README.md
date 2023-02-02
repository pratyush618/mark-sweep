# A C implementation of the mark-sweep algorithm for the capture of the used memory addresses during the creation of heap tree and using them as a reference for a new tree after dumping of the old heap tree.
## Quick Start

```console
$ make
$ ./heap
```

## Limitations

- The pointers to the heap can only be located in the heap and the stack.
- No packed structs. All of the pointers should be aligned.
- No tricks that obscure the pointers (like XOR Linked Lists).
- Never tested on other OS architectures excluding x86_64. Works fine on this one.
- Probably works only when compiled with GCC
