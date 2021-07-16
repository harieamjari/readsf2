# readsf2
Reads sf2 metadata

This software requires a little endian machine and a C compiler supporting
`#pragma pack(...)`. 

Some chunk in the sf2.1 specification where not implemented to recognize in this
implementation and stderr may scream. These chunks are from LIST-INFO:

```
[<irom-ck>] ; Refers to the Sound ROM Name
[<iver-ck>] ; Refers to the Sound ROM Version
[<ICRD-ck>] ; Refers to the Date of Creation of the Bank
[<IENG-ck>] ; Sound Designers and Engineers for the Bank
[<IPRD-ck>] ; Product for which the Bank was intended
[<ICOP-ck>] ; Contains any Copyright message
[<ICMT-ck>] ; Contains any Comments on the Bank
```

You may implement this on your own and create a pull request.
