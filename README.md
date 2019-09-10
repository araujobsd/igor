# igor (v.1.595)
Automated proofreader for text files, man pages, and DocBook SGML
source files.

## Description
igor proofreads documentation files to detect problems.  The goal is to
make formatting and problem detection easier, allowing the writer to
concentrate on the content.

Some tests can be performed on all files, while others are specific to
mdoc(7) or DocBook files.  igor uses file(1) to detect a file's type and
only runs the applicable tests on it.

Files compressed with gzip(1) or bzip(2) are automatically decompressed.
If multiple files are specified, filenames are displayed before each is
analyzed.  If no files are given, input is read from stdin.

By default, all tests are performed.  If options for individual tests are
given, only those tests will be done.  Several shortcut options make
testing common combinations easier; see the SHORTCUT OPTIONS section
below.

## How to use it?
```root# ./make-spelingwords```
```root# ./igor -R yourdoc.md```

## Authors
Warren Block ⟨wblock@FreeBSD.org⟩
