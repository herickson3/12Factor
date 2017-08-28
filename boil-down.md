What do they really mean?


Always assume you're on a fresh box


Don't write to disk


Read inputs from the environment


Write logs to stdout/stderr

note:
can I
- clone your repo
- run
  - install
  - test
  - build
  - start

Across writes that is
writing to disk is ok
- from one write to another is not
- it may not be there next time

Any long term data goes to a backing service
- DB, Cache, S3

