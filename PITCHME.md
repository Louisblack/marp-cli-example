---
marp: true
title: Quarkus
description: Hosting Marp slide deck on the web
theme: uncover
paginate: true
_paginate: false
---
![bg 40% opacity blur](./assets/quarkus.png)

# <!--fit--> Introduction to Quarkus

https://github.com/louisblack/quarkus-talk

---
![bg 40% opacity blur](./assets/kubernetes.png)

##### <!--fit--> A Kubernetes native framework

---

### ¯\\\_(ツ)\_/¯

* Microservice focused
* Containers not servers
* Creating and killing nodes all the time
* Scale out, not up

---
### How does it support this?

* Fast start up
* Low memory usage
* GraalVM Secret Sauce

---

### Tools we all know and love(ish)
* Dependency Injection
* JAX-RS (or Spring Web API)
* Vert.x (reactive API)
* JPA, Hibernate
* Etc.....

---

##### <!--fit--> Code!
---

![width:100%](./assets/graalvm.svg)
 
---
### Native Images

* Native binary (Linux 64 bit)
* Ahead of time compiled
* Statically linked
* Class initialisation at build time (Profiles for different environments)
* Ridiculous start up time
* Ridiculously low memory usage

---

##### <!--fit--> Demo!

---

Which opens the door to...

---

### Java on Lambda 😲

* Lambda API abstracted away - no events, etc
* Routing all done by the framework 

---

##### <!--fit--> Another Demo!

---
### Drawbacks :(

* Native images slow to create
* JVM tests fast but not the same as native
* Some libraries not compatible with AOT compilation
* `@RegisterForReflection` due to dead code removal
* SSL fiddly

---

Questions?

---
