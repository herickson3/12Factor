What are the 12 Factors?


Codebase 

note: one app = one codebase


Dependencies 

note: 
explicitly declare and isolate


Config 

note: 
store in the environment
config will change across deployments, but code will not


Backing Services 

note:
treat as attached resources
makes no distinction between local and 3rd party services


Build, Release, Run 

note:
strictly separate


Processes 

note: one or more stateless processes


Port Binding 

note:
exported services, completely self contained


Concurrency 

note:
scale horizontally


Disposability 

note:
fast startup & graceful shutdown
stopped or started at a moments notice


Dev/Prod Parity 

note:
as similar as possible


Logs

note:
stream logs to stdout/stderr


Admin Processes 

note:
one-off tasks
migrations

