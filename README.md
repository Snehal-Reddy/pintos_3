# Pintos - System Calls & User Programs

## How to running pintos on your machine?

$>need pintos (optional)

$>cd pintos/src/threads

$>make

$>cd build

$>pintos

## Running test cases:

$>pintos -v -k -T 60 --qemu --filesys-size=2 -p tests/userprog/args-none -a args-none -- -q -f run args-none 

### make check & make grade is build-in this operating system, you can running it by:

$>cd pintos/src/userprog

$>make check

$>make grade

## Test cases result:
pass tests/userprog/args-none

pass tests/userprog/args-single

pass tests/userprog/args-multiple

pass tests/userprog/args-many

pass tests/userprog/args-dbl-space

FAIL tests/userprog/halt

pass tests/userprog/exit

pass tests/userprog/create-normal

pass tests/userprog/create-empty

pass tests/userprog/create-long

pass tests/userprog/create-exists

pass tests/userprog/open-normal

pass tests/userprog/open-missing

pass tests/userprog/open-twice

pass tests/userprog/close-normal

pass tests/userprog/read-normal

pass tests/userprog/read-zero

pass tests/userprog/write-normal

pass tests/userprog/write-zero

pass tests/userprog/exec-once

pass tests/userprog/exec-multiple

pass tests/userprog/wait-simple

pass tests/userprog/wait-twice

22 of 23 tests passed.

## Files changed:
### /src/userprog/process.c
- changed process_execute
- changed start_process
- changed release_child
- changed process_wait
- changed process_exit
- changed setup_stack

### /src/userprog/syscall.c
- changed sys_haly
- changed sys_exit
- changed sys_exec
- changed sys_wait
- changed sys_create
- changed sys_remove
- changed sys_open
- added file_descriptor *lookup_fd
- changed sys_filesize
- changed sys_read
- changed sys_write
- changed sys_seek
- changed sys_tell
- changed sys_close

## All changed code is located between with following format:
/* My Code Begins */

CODES

/* My Code Ends */

## Data Structures:


## Algorithms:

