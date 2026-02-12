# Windows Executable Header Notes

The seemingly cryptic byte sequence `MZ` (often followed by a handful of
non-printable characters such as `0x90`) is a signature that identifies a file
as a DOS MZ executable, which also serves as the prefix for modern Portable
Executable (PE) binaries used on Windows. The initials refer to Mark Zbikowski,
one of the original architects of MS-DOS. When you encounter a binary that
starts with `4D 5A` (the hexadecimal values for `M` and `Z`), you can be
confident that it is intended to be executed by the Windows loader.

This repository collects small notes and experiments around binary formats.
