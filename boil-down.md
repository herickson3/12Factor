What do they really mean?


Always assume you're on a fresh box

note:
can I
- clone your repo
- run
  - install
  - test
  - build
  - start


Don't write to disk

note:
Across writes that is
writing to disk is ok
- from one write to another is not
- it may not be there next time
Any long term data goes to a backing service
- DB, Cache, S3


Read inputs from the environment


Write logs to stdout/stderr
