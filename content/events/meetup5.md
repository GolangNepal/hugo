---
title: "Golang Kathmandu Meetup #5 - Sep"
date: 2020-08-24T13:30:02+05:45
draft: true
---
### September 13 2020

---------

![Gopher](/gopher7.png)

# [**RSVP Here**](https://www.meetup.com/Golang-Kathmandu)
https://www.meetup.com/Golang-Kathmandu

-------------

### [Talk] No-instrumentation Log Injection in Go with eBPF

----


![Speaker](/speaker5.png)

Ishan Mukherjee
Co-founder: Pixie

**Developer Problem:**

Go programs are designed to be performant but we often don't have the right code-level instrumentation when a performance issue arises in a production go program. It's hard to predict where issues will arise and we can't instrument everything as over-aggressive instrumentation leads to maintenance overheads.

**Motivating Developer Experience:**

Enable tracing/logging of application code to answer the following questions without instrumentation:

Function Argument Tracing: "What are the arguments being passed to Foo(x, y, z)?"

Function Input-Output Tracing: "What are the arguments and return value of calls to Foo(x, y, z)?"

Conditional Function Tracing: "What are the arguments being passed to SetInfo(user, address) when user==alice?"

Function Latency Tracing (Profiling): "What is the latency (call to return) of calls to Login(username)?"

**Proposed Solution:**

Write and deploy eBPF userspace-probes native in Linux VMs v4.9+ to dynamically inject tracepoint in your go programs with the following constraints:
Less than 5% performance overhead

Reliably start, deploy and stop probes without leaks.

Provide apis to sample, filter and access data.

**Presentation Goals & Pixie's Involvement:**

Presentation would be about how go developers can independently write and deploy ann open-source eBPF probe without any back-end dependency. Pixie is one of many potential back-ends to allow developers to deploy such probes at scale. Other projects include BCC, inspector-gadget etc. - Speaker Bio: Ishan is the cofounder of Pixie, an SF based stealth auto-telemetry startup backed by Benchmark and Google Ventures. Teams like Disney use Pixie to access no-instrumentation (via eBPF), streaming & un-sampled telemetry to debug application performance issues without moving data out of their clusters. They're launching  on October  1st and are looking to engage with the golang developer community.

**References:**

India:  Zainab Bawa, Sayan  Chowdhury

US: Kelsey Hightower, Disney etc.

**Links:**

eBPF: https://ebpf.io/

Pixie: https://github.com/pixie-labs/pixie

Ishan's twitter: https://twitter.com/ishanmkh

----------

# [**RSVP Here**](https://www.meetup.com/Golang-Kathmandu)
https://www.meetup.com/Golang-Kathmandu
