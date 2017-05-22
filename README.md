# docker-compose-v3 with env file(s) example

## Usage
This repo is intended to show a simple example of using docker-compose version 3 with environment files to facilitate 
reuse based on external files without having to rewrite the compose file itself.  This is often helpful when deploying 
several containers together, either as a stack to a swarm or collection to an docker-engine.  A typical use case might 
be to have per-environment (e.g. Develop / test / prod) .env files containing appropriate settings (or have CI generate 
the file as part of a build)

## Notes
The default environment file is ".env", and this should be used for vars at the compose level.  Services have the
option to use the evn_file: key to specify file (or list) of environment variable files.


