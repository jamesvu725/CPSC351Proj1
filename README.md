# CPSC351Proj1
James Vu

1. Real time is the wall clock time. It is the elapsed time it takes from start to finish of the call. User time is the amount of CPU time spent in user space within the process. Sys time is the amount of CPU time spent in the kernel space within the process.
2. Sys time was longer than the user time. Sys time was longer because when we fork and get the child process to use execlp, the process goes from user space to kernel space to download the file. User time was shorter because we spent a small amount of time running the actual program's code. Most of the time spent was wget running in kernel space.
3. The parallel downloader is faster. When we are downloading multiple files, it is faster to download it in parallel instead of serial because serial works on one process at a time as oppose to parallel which works on multiple processes at a time.
4. Parallel downloader is noticably faster than the serial downloader when downloading multiple large files.
