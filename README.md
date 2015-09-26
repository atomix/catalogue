# Catalogue

[![Build Status](https://travis-ci.org/atomix/catalogue.png)](https://travis-ci.org/atomix/catalogue)

### [Website][Website] • [Google Group][Google group] • [Javadoc][Javadoc]

Catalog is a feature complete, fully asynchronous implementation of the [Raft consensus algorithm][Raft] in Java 8
designed for use in [Copycat][Copycat]. The implementation provides a fully featured [client][clients] and [server][servers]
and includes:
* Pre-vote election protocol ([4.2.3][dissertation])
* Session-based linearizable writes ([6.3][dissertation])
* Lease-based reads from leaders ([6.4.1][dissertation])
* Serializable reads from followers ([6.4.1][dissertation])
* Session-based state machine events ([6.3][dissertation])
* Membership changes ([4.3][dissertation])
* Log compaction via cleaning ([5.3][dissertation])

Additionally, this implementation has undergone [Jepsen testing](http://github.com/jhalterman/copycat-jepsen)
to verify it maintains linearizability in a number of different failure scenarios.

*For more information on the Raft implementation itself, see [Raft internals](http://atomix.github.io/copycat/user-manual/raft-internals/)*

[Raft]: https://raft.github.io/
[dissertation]: https://ramcloud.stanford.edu/~ongaro/thesis.pdf
[Copycat]: http://github.com/atomix/copycat
[clients]: http://atomix.io/user-manual/raft-internals/#clients
[servers]: http://atomix.io/user-manual/raft-internals/#servers
[Website]: http://atomix.io/user-manual/raft-framework/
[Google group]: https://groups.google.com/forum/#!forum/copycat
[Javadoc]: http://atomix.io/catalogue/api/latest/
