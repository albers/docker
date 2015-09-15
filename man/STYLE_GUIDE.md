Manual Page Style Guide
=======================

This page describes how to format the Docker Unix manual pages.
These pages are written in Markdown, see [README.md](README.md) for how to
generate and view the corresponding manual pages.

## Synopsis

The command, its options and arguments. Optional elements in [square brackets],
alternatives separated by "|", repeated elements followed by three dots (...).
No default values.

Command and options in **bold**, placeholders (variables) uppercase and *italics*.
Literals in *italics*, quoted if they look like placeholders.

One argument/option per line, not indented, no blank lines.

### Boolean options

legal syntax: `--option`, `--option=true`, `--option=false`,
but *not* `--option true` or `--option false` (this is different from most
Unix commands).

They are formatted as follows:

#### A boolean option defaulting to `false`

    [**--option**]

#### A boolean option defaulting to `true`

    [**--option**=*false*]

### Options with arguments

legal syntax: `--option=argument`, `--option argument`.

They are formatted as follows:

#### An option that may appear only once

    [**--option**[=]*ARGUMENT*]

#### An option that may appear multiple times

    [**--option**[=]*ARGUMENT*]...

