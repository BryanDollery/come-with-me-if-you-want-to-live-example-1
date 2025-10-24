---
spec_order: 2 of 4
required: true
preceded_by:
 - @spec/01 - spec.md
followed_by:
 - @spec/03 - coding-standards.md
---

# Architecture

Security is the top priority
This is a gitops monorepo automated by makefile, bash, kustomize, and tekton
Never ‘summarize’ the specifications themselves or the code
You must use the calculator tool when performing any arithmetic
Server
XAPI, PAPI, and SAPI layers
The backend is an event-driven DDD with CQRS written in Bun
Postgresql is the only db we use, RedPanda is the only bus
We run on kubernetes in the cloud
All 3rd party components are open-source
The UI is a react SPA

# Models
@spec/model/components.puml

