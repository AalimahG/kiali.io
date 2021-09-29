---
title: "Concepts"
date: 2018-06-20T19:04:38+02:00
draft: false
weight: 1
---

### Application

Is a logical grouping of [Workload]({{< relref "#workload" >}})s defined by the application labels that users apply to an object. In Istio it is defined by the [Label App]({{< relref "#label-app" >}}). [Istio Label Requirements](link:https://istio.io/docs/setup/kubernetes/spec-requirements/).

### Application Name

It's the name of the [Application]({{< relref "#application" >}}) deployed in your environment. This name is provided by the [Label App]({{< relref "#label-app" >}}) on the [Workload]({{< relref "#workload" >}}).

### Deployment

A deployment is a replication controller based on a user defined template called a [Deployment](https://kiali.io/documentation/latest/glossary/concepts/#_deployment) configuration. Deployments are created manually or in response to triggered events.

### Istio object/configuration Type

This is the type specified in the Istio Config. This could be any of the following types: Gateway, [Virtual Service]({{< relref "#virtual-service" >}}), DestinationRule, ServiceEntry, Rule, Quota or QuotaSpecBinding.

### Istio Sidecar

For more information see the [Istio Sidecar]({{< relref "#istio-sidecar" >}}) definition in [Istio Sidecar Documentation](link:https://istio.io/v1.5/docs/reference/commands/sidecar-injector/).

### Label

It's a user-created tag to identify a set of objects.

An empty [label selector](link:https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/) (that is, one with zero requirements) selects every object in the collection.

A null [label selector](link:https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/) (which is only possible for optional selector fields) selects no objects.

For example, Istio uses the [Label App]({{< relref "#label-app" >}}) & [Label Version]({{< relref "#label-version" >}}) on a [Workload]({{< relref "#workload" >}}) to specify the version and the application.

### Label App

This is the 'app' label on an object. For more information, see [Istio Label Requirements](https://istio.io/docs/setup/kubernetes/spec-requirements/).

### Label Version

This is the 'version' label on an object. For more information, see [Istio Label Requirements](https://istio.io/docs/setup/kubernetes/spec-requirements/).

### Namespace

Namespaces are intended for use in environments with many users spread across multiple teams, or projects.

Namespaces are a way to divide cluster resources between multiple users.

### Quota

A limited or fixed number or amount of resources.

### ReplicaSet

Ensures that a specified number of pod replicas are running at any one time.

### Service

A [Service]({{< relref "#service" >}}) is an abstraction which defines a logical set of Pods and a policy by which to access them.  A Service is determined by a [Label]({{< relref "#label" >}}).

### Service Entry

For more information see the [Service Entry]({{< relref "#service-entry" >}}) definition in [Istio Service Entry Documentation](link:https://istio.io/docs/reference/config/networking/service-entry).

### VirtualService

For more information see the [Virtual Service]({{< relref "#virtual-service" >}}) definition in [Istio VirtualService Documentation](link:https://istio.io/docs/reference/config/networking/virtual-service).

### Workload

For more information see the [Istio Workload definition](link:https://istio.io/help/glossary/#workload).

### Workload Type

It's the type of the [Workload]({{< relref "#workload" >}}), Kiali currently supports the [Deployment]({{< relref "#deployment" >}}) type.