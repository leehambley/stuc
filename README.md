# Description

*stuc* manages configuration settings.  Its purpose is to have a
single, universal interface for reading configuration settings.

Software configuration is usually stored in some kind of hierarchical
data structure, encoded as plain text file.  Various encodings exist
and are used for this (e.g. `ini' files, `yaml', `json').  Working
with any of these files requires decoding the text file back into a
hierarchical data structure that the processing program understands.
The programming libraries for this vary in their semantics, robustness
and availability for different programming languages.

The type of data that can be encoded is also limited, depending on the
encoding.  Some encodings (or implementations of such) support
substituting environment variables, including other files or other
means of aggregating data from other sources.

The filesystem already provides a hierarchical data store and requires
no special tools beyond read/write access to files.  Executable files
allow dynamic query/generation of values.  *stuc* provides an
interface for querying configuration settings in a structured manner.

# Requirements

*stuc* is written in POSIX C (200809) and thus should compile and run on
POSIX compatible systems.  It only calls external utilities that are
specified in POSIX.

# Author

Dario Hamidi, 2013, [Github](https://github.com/dhamidi/stuc)

# License

All code is licensed under the
[GNU GPL](http://www.gnu.org/licenses/gpl.html).  Documentation is
licensed under the [GNU FDL](http://www.gnu.org/copyleft/fdl.html).
