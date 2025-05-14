Old school days, DOS ( MS-DOS / IBM PC-DOS ) is single task.
I created a concept C program to schedule multi-process on DOS:
print_ticks() is setup in main(), and scheduled in int 0x8,
and after print_ticks() is done, return control to main().
A video of the program is at
https://drive.google.com/file/d/1X95Lhqbfal2Y4i3Zv9AVMHq2Dha44Zb9/view?usp=drive_link

In this repo, there are outline for C/Pascal code.
And MPROC.EXE/PCCL.EXE for MS-DOS built from C/Pascal.
MPROC.C/PCCL.PAS are not published.

PCCL.EXE schedule proc19 in timer interrupt.
When hit Esc, proc19 will return to main program pccl.
pccl will call proc19 again.
Hit Esc, program then ends.
Video is here:
https://drive.google.com/file/d/1EwvvL6YkWh2nDBKI5VTPtT6efRvOMQSj/view?usp=drive_link
