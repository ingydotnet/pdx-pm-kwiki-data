## March2010Meeting

    Wed. March 10th, 6:53pm at FreeGeek -- 1731 SE 10th Ave.

### How to learn to parse huge XML documents by doing it wrong for 5 years

Video of lecture: http://www.ustream.tv/recorded/5349583

Speaker: Tyler Riddle

When XML documents can't fit into memory the vast majority of solutions available on CPAN are no longer available to you; when the XML documents are so large they take up to 16 hours to process with the standard tools for handling large documents your hands are tied even more. Tyler will cover his learning experiences creating the [Parse::MediaWikiDump](http://search.cpan.org/dist/Parse-MediaWikiDump) and [MediaWiki::DumpFile](http://search.cpan.org/dist/MediaWiki-DumpFile) modules which are made to handle the 24 gigabyte English Wikipedia dump files in a reasonable time frame.

1) Real world benchmarks of C and perl libraries used to process huge XML documents.

2) The dirty little secret about XS and what it means for you in this context.

3) The evolution of the implementation of a nice interface around event oriented (SAX style) XML parsing.

4) Why [XML::LibXML::Reader](http://search.cpan.org/~pajas/XML-LibXML-1.70/lib/XML/LibXML/Reader.pod) and [XML::CompactTree](http://search.cpan.org/dist/XML-CompactTree) are your friends and how to tame them.
