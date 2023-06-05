# .esar ECMAScript Archive
A ECMAScript Archive is like .phar and .asar a Archive format as it is designed to be archive able while this term
is a bit confusing when talking about AwesomeOS it got designed for interop with legacy systems and to teach developers
about the concepts of a transport and archive format. 

see: ./tar.md

for internals. 

It gets loaded mainly via a esar format supporting loader function. That takes the stub and creates a runable function
out of it and then throws the data as arrgument into the created function.
