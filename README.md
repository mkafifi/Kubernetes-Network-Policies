# Kubernetes Network Polices

First : Deny all traffic (Ingress and Egress) to all pods 
```
# Deny All Network Policy for Namespace
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
