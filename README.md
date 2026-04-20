# Container Documentation for MetalLB-Controller

MetalLB controller container provides Layer 2 and BGP-based load balancing functionality for bare metal Kubernetes clusters. It enables LoadBalancer service types in environments without cloud provider integration, offering enterprise-grade network load balancing capabilities with high availability and automatic failover features.

## Key Features

Core capabilities and strengths of this container

- Layer 2 and BGP mode support for network load balancing
- Automatic IP address management and allocation
- High availability configuration with leader election
- Native Kubernetes integration for LoadBalancer services

## Common Use Cases

Typical scenarios where this container excels

- Bare metal Kubernetes cluster load balancing
- On-premises data center service exposure
- Edge computing network management
- Multi-cluster service load balancing

## Pull Latest Image

Download the container image from the registry
```bash
docker pull ghcr.io/cleanstart-containers/metallb-controller:latest
```
```bash
docker pull ghcr.io/cleanstart-containers/metallb-controller:latest-dev
```

## Basic Run

Run the container with basic configuration
```bash
docker run -it --name metallb-controller-test ghcr.io/cleanstart-containers/metallb-controller:latest-dev
```

## Production Deployment

Deploy with production security settings
```bash
docker run -d --name metallb-controller-prod \
  --read-only \
  --security-opt=no-new-privileges \
  --user 1000:1000 \
  ghcr.io/cleanstart-containers/metallb-controller:latest
```
## Documentation Resources
Essential links and resources for further information
 
**CleanStart Images**: https://images.cleanstart.com/
 
**Community Images**:
**Docker Hub**: https://hub.docker.com/u/cleanstart<br>
**GitHub**: https://github.com/cleanstart-containers<br>
**AWS ECR Public Gallery**: https://gallery.ecr.aws/cleanstart/
 
**Presence on Social Media**:
**Community**: https://www.linkedin.com/groups/18324021/<br>
**YouTube**: https://www.youtube.com/@CleanStartOfficial<br>
 
**Contribute to Container Use Cases**: https://github.com/cleanstart-dev/cleanstart-use-cases/
