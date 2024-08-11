# MEMDEBUG
A little memory debugger.
The debugger aliases malloc and free to its own malloc and free that call the stdlib versions but also saves the file and line.
You can use `memdebug_view()` to display all allocations that werent freed and where they were allocated. 

# USAGE
Have `memdebug.h` in your include path and compile with `memdebug.c`.
Remember to initialize memdebug by calling init_memdebug()
and clean up memdebug with cleanup_memdebug()