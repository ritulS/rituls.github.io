---
title: "Mewbie: Scale Adjustable Benchmark for Microservice Deployments"
excerpt: "INESC-ID Lisbon, Vrije Universiteit; Supervisors: Rodrigo Rodrigues, Alexandru Iosup <br/><img src='/images/mewbie_high_level.png'>"

collection: portfolio
---

Microservice architectures became essential for large-scale services, powering platforms like Meta, Uber and Netflix. While they offer advantages in scalability and agility, their inherent complexity and massive scale make it almost impossible to understand the performance implications of system design choices, particularly when system designers do not have access to production environments. Furthermore, while a few microservice benchmarks exist, they fall short of this goal as they are based on simplified applications, orders of magnitude smaller than real-world deployments. This forces developers to rely on an overly simplistic testing approach, limiting their ability to assess performance in more realistic environments.

We present Mewbie, the first scale-adjustable benchmark that leverages production traces enriched with essential details like object identifiers and read-write ratios, to create flexible and representative microservice workloads. Mewbie is able to scale to any deployment size through a novel trace downscaling technique that preserves key topological features of the original call graph, enabling scalable benchmarking without the overhead of a full-scale deployment.
<!-- %, allowing users to create applications that fit their desired size -- while still being representative of real-world applications. -->

We showcase Mewbie with a datastore-focused use case, where we experiment with how a microservice deployment based on the Alibaba production dataset responds to different datastore mixtures (using Redis, MongoDB and MySQL), and also the impact of using different consistency semantics. Our evaluation shows that Mewbie effectively captures the dynamics of large-scale microservice infrastructures, and provides useful insights regarding how system design choices affect the end-to-end request processing time.
