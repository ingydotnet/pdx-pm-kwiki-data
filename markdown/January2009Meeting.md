# How a Virtual Machine Works

**[[chromatic]]** presents:

Perl 6, Perl 5, Python, Ruby, Lua, JavaScript, Java, C#, and many other
languages use virtual machines as their execution environments.  Instead of
compiling directly to machine code, they rely on the presence of an ideal
machine built specifically for the language -- porting the language to a new
architecture often means only porting that virtual machine.

Does that sound complicated?  It's not.  Some of the details of very efficient
and effective virtual machines are, but the general ideas are simple.

This talk explains the important components of a virtual machine and how they
fit together.  Examples will come from the world of Perl 5, Parrot, and Perl
6, but the concepts apply to many languages and VMs.

You may never need to hack the guts of your favorite language, but
understanding how they work can help you become a better programmer.

Pictures: http://flickr.com/photos/28801292@N05/3199149426/

We sure did talk a bunch about [[GoogleSummerOfCode2009]]
