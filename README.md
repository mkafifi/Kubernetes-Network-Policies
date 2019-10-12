# k8s-network-policies
Kubernetes Network Polices

First : Deny all traffic (Ingress and Egress) to all pods 
```
# Deny All Network Policy for the Blue Namespace
apiVersion: networking.k8s.io/v1
kind: NetworkPolicy
metadata:
  name: default-deny
spec:
  podSelector: {}
  policyTypes:
    - Ingress
  matchLabels: {}
  ```
