+++
author = "David Stacy"
title = "A Cloud Operating System?"
date = "2021-07-18T10:52:59+08:00"
description = "Can we make public cloud easy to manage?"
comment = true
+++

Any small, medium, or large enterprise contemplating the use of public
cloud will need an operating system for that cloud.  Not an operating
system for virtual servers in the cloud, we already have that, it’s
called Linux (in various flavors).  Enterprises need an operating
system for cloud resources that does what operating systems do for
personal computers, connect all the hardware so applications can run.

But isn’t that the promise of Kubernetes and all of the other myriad
of container + cloud platforms?  And yes, for all applications that
can run in Kubernetes you can spin up a platform on any cloud and be
fully ready to run.  But most enterprises have legacy apps, that can,
and maybe should also move to the cloud.  Sometimes for good,
sometimes until either retirement or they can be modernized.  What do
we do with those?

In the late 90’s and up to the time of .Net, a Windows developer had
several levels of Operating System calls to work with including INT
21h for a virtual dos machine for legacy apps.  The Windows API had
several levels of system calls and services, base calls, Win16, Win32.
If you didn’t want to talk to those directly, you could use wrapper
classes (now a higher level) such as MFC for C++ or the Windows
Template Library, and Windows kept coming out with more including OLE,
COM, and the .NET Framework.  All in the same system.  All
applications using different API’s and wrappers could simultaneously
operate side by side if they were well-behaved.

The Operating System Analogy helps to remind us that a successful OS
allowed legacy apps direct hardware level access to the CPU, any
successful Cloud Operating System will need to allow existing
applications direct access to the resources they need like virtual
servers, databases of the relational variety, and block storage
directly mounted to the virtual server, just like they were used to
when the apps were first designed, coded and built.  Cloud Operating
Systems should not leave these apps behind.

A successful cloud OS will be multilane, and include paths for legacy
applications, including three tier server-based apps, container-based
apps, serverless, microservice architectures, and maybe some more we
haven’t thought of yet.  The cloud operating system will be one
system, including base services that all applications need, like calls
for access to base resources such as compute, storage, data, network,
and include in that system centralized, security, identity,
networking, and include standard ways to package and deploy
applications just like operating systems have installers.  In fact,
most mature operating systems are easily installable and pre-loaded
themselves, so perhaps our cloud operating system should be as well.

We’re not there yet, in a future blog let’s talk about what actually
happens today, and how close or far we are from this ideal, one system
for all applications.
