# K8s From-Ground-Up

For a better understanding of each aspect of spinning up a Kubernetes cluster, we will do it without any automated helpers. You will install each and every component manually from scratch and learn how to make them work together.

## Let us begin!!! 

**Step One: INSTALL CLIENT TOOLS BEFORE BOOTSTRAPPING THE CLUSTER.**

- Aws CLI - is a unified tool to manage your AWS services.
- Kubectl - this command line utility will be your main control tool to manage your K8s cluster.
- cfssl - an open source toolkit for everything TLS/SSL from Cloudflare
- cfssljson -  a program, which takes the JSON output from the cfssl and writes certificates, keys, CSRs, and bundles to disk.

Installing kubectl

```bash
#Download the binary
wget https://storage.googleapis.com/kubernetes-release/release/v1.21.0/bin/linux/amd64/kubectl

# Make it executable
chmod +x kubectl

#Move to the Bin directory
sudo mv kubectl /usr/local/bin/

# Verify that kubectl version 1.21.0 or higher is installed:
kubectl version --client
```

![kubectl installation](./images/1.png)