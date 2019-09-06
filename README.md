# Mojang2Tsrg
A small tool that converts Mojang's ProGuard obfuscation map to TSRG format, for use by SpecialSource

It is currently under development, but is minimally functional. Providing the proguard .txt as the first argument,
and the output .tsrg as the second argument, it does exactly what it says.

## Notice
When I run the generated mappings with SpecialSource, I get a NullPointerException on `remapJar`.  I have yet
to determine if that is an issue with SpecialSource or the mappings that are generated by this application.  I
do know that these mappings are correct TSRG format, so it could be the inclusion of extra classes or fields
that may be the issue.

However, to fix this issue, use SpecialSource release 1.8.4 or lower.  They apply without error on that version.
