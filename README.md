# stats-slurm
Scripts (and soon, possibly, notes) for working with the departmental Slurm servers.

`interactive_session` is a script that I keep in my `~/bin/` directory which, crucially, is in my `PATH`.
It is a very basic script that will start an interactive/debug session on a partition of your choice if you
 are logged into a slurm head node.  Example use:

```
interactive_session -p <partition_name>
```
This will start a 30 minute (the current departmental limit) debug session in a sensible file location.
The script will attempt to throw informative errors if, for example, you are not logged into a slurm head node,
 or you enter a <partition_name> which is not recognised.  If you miss the `-debug` suffix then this will be appended for you.


# Useful Slurm references:
- [Official Slurm documentation website](https://slurm.schedmd.com) (from schedmd)
  - [schedmd slurm cheatsheet](https://slurm.schedmd.com/pdfs/summary.pdf)
- [Princeton Research Computing Slurm Documentation](https://researchcomputing.princeton.edu/support/knowledge-base/slurm)
- [Arctic University of Norway HPC documentation](https://hpc-uit.readthedocs.io/en/latest/jobs/examples.html)
- [University of Florida Research Computing Help](https://help.rc.ufl.edu/doc/UFRC_Help_and_Documentation)
- [University of Kansas help page](https://crc.ku.edu/hpc/how-to#script)

If you're in Oxford's department of statistics, the following link may be useful:
- [Oxford Statistics internal Slurm documentation](http://internal.stats.ox.ac.uk/it-support/computation/slurm/)