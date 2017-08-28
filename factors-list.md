What are the 12 Factors?


Codebase | one app = one codebase


Dependencies | explicitly declare and isolate


Config | store in the environment

note:
config will change across deployments, but code will not


Backing Services | treat as attached resources

note:
makes no distinction between local and 3rd party services


Build, release, run | strictly separate

note:
build - include / bundle all dependencies & create executable

release - add any relevant config / backing services

run - start up a release

Build + config = release

releases are append only

builds initiated by developers. runs happen automatically by platform


Processes | stateless


Port binding | exported services

note:
completely self contained


Concurrency | scale horizontally


Disposability | fast startup & graceful shutdown

note:
stopped or started at a moments notice


Dev/prod parity | as similar as possible


Logs | stream stdout / stderr


Admin processes | one-off tasks

