# perf annotate

## SYNOPSIS
```
perf annotate [-i <file> | --input=file] [symbol_name]
```

## OPTIONS
```
    -i, --input=
        Input file name. (default: perf.data unless stdin is a fifo)

    -d, --dsos=<dso[,dso...]>
        Only consider symbols in these dsos.

    -s, --symbol=<symbol>
        Symbol to annotate.

    -f, --force
        Don’t complain, do it.

    -v, --verbose
        Be more verbose. (Show symbol address, etc)

    -D, --dump-raw-trace
        Dump raw trace in ASCII.

    -k, --vmlinux=<file>
        vmlinux pathname.

    -m, --modules
        Load module symbols. WARNING: use only with -k and LIVE kernel.

    -l, --print-line
        Print matching source lines (may be slow).

    -P, --full-paths
        Don’t shorten the displayed pathnames.

    --stdio
        Use the stdio interface.

    --tui
        Use the TUI interface. Use of --tui requires a tty, if one is not present, as when piping to other
        commands, the stdio interface is used. This interfaces starts by centering on the line with more
        samples, TAB/UNTAB cycles through the lines with more samples.

    --gtk
        Use the GTK interface.

    -C, --cpu
        Only report samples for the list of CPUs provided. Multiple CPUs can be provided as a comma-separated
        list with no space: 0,1. Ranges of CPUs are specified with -: 0-2. Default is to report samples on
        all CPUs.

    --asm-raw
        Show raw instruction encoding of assembly instructions.

    --source
        Interleave source code with assembly code. Enabled by default, disable with --no-source.

    --symfs=<directory>
        Look for files with symbols relative to this directory.

    -M, --disassembler-style=
        Set disassembler style for objdump.

    --objdump=<path>
        Path to objdump binary.

    --skip-missing
        Skip symbols that cannot be annotated.

    --group
        Show event group information together
```