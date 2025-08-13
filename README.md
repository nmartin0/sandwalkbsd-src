SandwalkOS is a BSD derivative. This OS will strive to be compliant with the
recent POSIX and C standards. With discretion, features extraneous to the core
functioning of the system which is defined in terms of core functionality of the
system as well as standards compliance are likely to be removed except in
extraordinary circumstances. Priorities beyond this include code quality and
development ease. This system should have minimal dependencies, and newly added
files should be licensed under compatible permissive licensing. Licensing which
changes this should not be included within the kernel, and only within
applications where critical functionality relating to a tool and its POSIX
compliance are isolated and considered interim until a permissive rewrite
exists. System tooling should be minimal, and as with the kernel and libraries,
either provide standards compliance, essential system functionality, or provide
an extraordinary service which can justify its inclusion.

Development is to occur within at least four branches; one local, and three
remote. Initial development should occur within a local branch to a
modification. This modification should compile afresh, the resulting OS should
boot, and the feature should to tested. Once the modification is considered to
not be broken, a request to merge it to remote branch alpha should be made. A
merge request is not a guarantee that the feature will be accepted. Changes to
the system should fall into one of the following reasons; update to standards
compliance, update to system performance, polishing of code, addition and/or
modification of comments, or removal of non-essential functionality. While there
are exceptions to these general guidelines, many features falling outside of
those boundaries should be created and maintained in a downstream variant of the
OS. Remote branch alpha contains unstable modifications -- though unstable, these
should be functional. Once stable, these changes might be merged into remote
branch beta. Remote branch beta should contain stable changes which have been
thoroughly tested, where the relevant source code supporting such changes has
been documented thoroughly, and the code has been written cleanly. Branch beta
is effectively the stable development branch from which the release branch
occasionally branches from. The release branch is to be forked from branch beta,
and modifications to the release branch should be limited to critical fixes. 

A standard C toolchain as well as basic tooling to receive additional software
via remote sources should always be available. 

This system should be fully capable and usable on its own. Its focus on
cleanliness and minimality should lend it well to downstream development. This
project is designed to address my own observations in deficiencies in a generic,
minimal OS that supports standards compliance, minimality, while also being
modern and fully functional as a standard OS.
