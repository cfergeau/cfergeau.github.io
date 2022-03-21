---
title: "My First Post"
date: 2022-02-06T16:20:50+01:00
authors:
  - cfergeau
draft: true
---

This is a code test
{{< highlight go "linenos=table" >}}
import "libvirt.org/go/libvirtxml"

func addVSock(domain *libvirtxml.Domain) {
	domain.Devices.VSock = &libvirtxml.DomainVSock{
		Model: "virtio",
		CID: &libvirtxml.DomainVSockCID{
			Auto: "yes",
		},
	}
}
{{< /highlight >}}

{{< mermaid class="text-center">}}
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
{{< /mermaid >}}

```golang
import "libvirt.org/go/libvirtxml"

func addVSock(domain *libvirtxml.Domain) {
	domain.Devices.VSock = &libvirtxml.DomainVSock{
		Model: "virtio",
		CID: &libvirtxml.DomainVSockCID{
			Auto: "yes",
		},
	}
}
```

and let's also try some XML
```xml
<vsock model='virtio'>
    <cid auto='yes'/>
</vsock>
```


This is a test
* enum #1
* enum #2
* enum #3

