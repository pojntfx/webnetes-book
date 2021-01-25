# Introduction

Webnetes is a peer-to-peer computing platform for the browser and node. Unlike traditional, server-only container orchestration systems such as [Kubernetes](https://kubernetes.io/), which usually use [OCI Containers](https://opencontainers.org/) for compute, [CNI](https://github.com/containernetworking/cni) for networking and [CSI](https://github.com/container-storage-interface/spec) for storage, Webnetes switches these components out in favor of [WebAssembly](https://en.wikipedia.org/wiki/WebAssembly), [WebRTC](https://en.wikipedia.org/wiki/WebRTC) and [WebTorrent](https://en.wikipedia.org/wiki/WebTorrent). By doing so, Webnetes is **universal** — it runs on every system, from the server (using [Node](https://nodejs.org/en/)) to the browser.

By using standardized web APIs and polyfilling APIs that would normally only be found on the server (such as [Berkeley sockets](https://en.wikipedia.org/wiki/Berkeley_sockets)) to work everywhere, Webnetes is able to bridge the gap between devices. It even runs on iOS (using Safari) and other heavily restricted proprietary mobile operating systems, without requiring any installation. Joining a cluster becomes as easy as scanning a QR code or clicking a link; no need for proprietary app distribution mechanisms like the App Store or the Play Store. Many workloads can thus also be moved from the server to the client, removing the dependency on expensive servers or proprietary cloud systems such as AWS or GCP.

Due to recent advancements to the web platform, apps are no longer limited to only using JavaScript — Webnetes uses WebAssembly, which means that many languages, including C, C++, Go, Rust and Java, are supported. You also aren't limited to apps without native capabilities either; almost all web APIs are available, including [Web Bluetooth](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API), [Web USB](https://developer.mozilla.org/en-US/docs/Web/API/USB), [Web MIDI](https://www.w3.org/TR/webmidi/), [File System Access](https://developer.mozilla.org/en-US/docs/Web/API/File_System_Access_API) and many more. In most cases, getting an app to run in Webnetes simply means to recompile to WebAssembly. Even software that depends on lower-level networking (such as TCP client/server systems) or terminals runs effortlessly. Thanks to the power of WebRTC, typical networking barriers in building distributed apps are also removed; Webnetes creates global peer-to-peer overlay networks, removing the need for complex and expensive VPN or tunneling setups.

Ready to learn how to use Webnetes? Continue to the [getting started guide](./getting-started)!