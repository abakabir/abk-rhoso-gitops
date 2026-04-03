rhoso-gitops/
├── 01-prerequisites/         # Tout ce dont OCP a besoin (Operators infra)
│   ├── kustomization.yaml
│   ├── nmstate/
│   ├── metallb/
│   └── cert-manager/
├── 02-operators/             # Les opérateurs RHOSO spécifiques
│   ├── kustomization.yaml
│   └── openstack-operator/
├── 03-config/                # La configuration réelle (CRs)
│   ├── control-plane.yaml
│   ├── data-plane.yaml
│   └── networking.yaml
└── apps/                     # Les manifests ArgoCD (si utilisé)
    ├── prerequisites-app.yaml
    └── rhoso-app.yaml
