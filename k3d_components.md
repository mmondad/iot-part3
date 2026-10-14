K3d is primarily a single CLI executable, named k3d, but internally its code is organized into multiple packages and components.

k3d executable
│
├── CLI layer
│   └── Parses commands and flags
│
├── Cluster management logic
│   ├── Cluster configuration
│   ├── Node lifecycle management
│   ├── Load-balancer configuration
│   ├── Registry configuration
│   └── Readiness checks
│
├── Container runtime integration
│   ├── Docker API communication
│   ├── Container operations
│   ├── Network operations
│   └── Port mapping
│
└── Kubeconfig management
    └── Kubernetes client configuration