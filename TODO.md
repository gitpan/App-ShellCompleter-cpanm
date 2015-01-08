* TODO [2015-01-08 Thu] _cpanm: replace XPAN::Query with an external service (probably need to setup this service)

  - MetaCPAN (MetaCPAN::Client), while powerful and adequate, is not optimal for
    this task. the response time is rather slow (1.5s+) and returns too much data.
    ideally we only want something that returns list of PAUSE ids, package names,
    dist names.
  - CPANDB is also not ideal because, like XPAN::Query, it downloads the whole
    index first.
