# Sagano

For many years, we've had Linux and containers operating in connected but
separate worlds.  Today, we are excited to announce that we are bringing these
worlds together.  We're making the ecosystem of content available to you in
containers, now to your core Linux systems.  Containers now become the language
for building the OS.  Boot them to your core Linux systems.  Modify them in a
Containerfile/Dockerfile.  Whether standalone images to modify as you see fit in
your datacenter, immutable images at the edge or worker nodes in
Kubernetes/OpenShift - one, consistent approach.  We're always striving to make
developing applications across the hybrid cloud easier and to make your IT
landscape easier to manage even as you face increasing complexity.  And we hope
you are as excited about this as we are.

## Goals

This project's toplevel goal is to create "base" *bootable* container images
from Fedora ELN and CentOS Stream packages.

## Trying it out

See [install.md](./install.md).

## Status

This is an in-development project not intended for production use yet.

## Differences from Fedora CoreOS

Fedora CoreOS today is not small; there are multiple reasons for this, but
primarily because it was created in a pre-bootable-container time.  Not everyone
wants e.g. moby-engine.

But going beyond size, the images produced by this project will focus
on a container-native flow.  We will ship a (container) image that does not
include Ignition for example.

## Differences from RHEL CoreOS

We sometimes say that RHEL CoreOS [has FCOS as an upstream][1] but this is only
kind of true; RHEL CoreOS includes a subset of FCOS content, and is lifecycled
with OCP.

An explicit goal of this project is to produce bootable container images
that can be used as *base images* for RHEL CoreOS; for more on this, see e.g.
<https://github.com/openshift/os/issues/799>

## Differences from RHEL for Edge

It is an explicit goal that Sagano also becomes a "base input" to RHEL for Edge.

## What does Sagano means

From [Wikipedia](https://en.wikipedia.org/wiki/Bamboo_Forest_(Kyoto,_Japan)):

> Bamboo Forest, Arashiyama Bamboo Grove or Sagano Bamboo Forest, is a natural
> forest of bamboo in Arashiyama, Kyoto, Japan

[1]: https://github.com/openshift/os/blob/master/docs/faq.md#q-what-is-coreos
