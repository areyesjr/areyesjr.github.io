---
layout: default
---

### Doctl

#### Cheat sheet

[Droplets](https://www.digitalocean.com/products/droplets/)

Create droplet:  
```doctl compute droplet create <dropletname> --size "s-1vcpu-1gb" --image "centos-7-x64" --region "lon1"
```

List droplets:
```doctl compute droplet list```

Delete droplet:  
```doctl compute delete <dropletid>```

List neighbors: (if your droplets are running on same hypervisor)  

```doctl compute droplet neighbors <dropletid>```

List snapshots for droplet:  

```doctl compute droplet snapshots <dropletid>```

[DO Kubernetes](https://www.digitalocean.com/products/kubernetes/)

Create DO kubernetes cluster:  

```doctl k8s cluster create <clustername> --count 3 --region sfo2```

List kubernetes clusters:  

```doctl k8s cluster list```

Delete kubernetes cluster:  

```doctl k8s cluster delete <clustername>```

More to come..........


[..](../)

You can follow me on [twitter](https://twitter.com/AlexisReyesJR).
