## OWASP Cloud-Native Application Security Top 10

CNAS-1: Insecure cloud, container or orchestration configuration

Examples:

    Publicly open cloud storage buckets
    Imrpoper permissions set on cloud storage buckets
    Container runs as root
    Container shares resources with the host (network interface, etc.)
    Insecure Infrastructure-as-Code (IaC) configuration
    …

CNAS-2: Injection flaws (app layer, cloud events, cloud services)

Examples:

    SQL injection
    XXE
    NoSQL injection
    OS command injection
    Serverless event data injection
    …

CNAS-3: Improper authentication & authorization

Examples:

    Unauthenticated API access on a microservice
    Over-permissive cloud IAM role
    Lack of orchestrator node trust rules (e.g. unauthorized hosts joining the cluster)
    Unauthenticated orchestrator console access
    Unauthrized or overly-permissive orchestrator access

CNAS-4: CI/CD pipeline & software supply chain flaws

Examples:

    Insufficient authentication on CI/CD pipeline systems
    Use of untrusted images
    Use of stale images
    Insecure communication channels to registries
    Overly-permissive registry access
    Using a single environment to run CI/CD tasks for projects requiring different levels of security
    …

CNAS-5: Insecure secrets storage

Examples:

    Orchestrator secrets stored unencrypted
    API keys or passwords stored unencrypted inside containers
    Hardcoded application secrets
    Poorly encrypted secrets (e.g. use of obsolete encryption methods, use of encoding instead of encryption, etc.)
    Mounting of storage containing sensitive information
    …

CNAS-6: Over-permissive or insecure network policies

Examples:

    Over-permissive pod to pod communication allowed
    Internal microservices exposed to the public Internet
    No network segmentation defined
    End-to-end communications not encrypted
    Network traffic to unknown or potentially malicious domains not monitored and blocked
    …

CNAS-7: Using components with known vulnerabilities

Examples:

    Vulnerable 3rd party open source packages
    Vulnerable versions of application components
    Use of known vulnerable container images
    …

CNAS-8: Improper assets management

Examples:

    Undocumented microservices & APIs
    Obsolete & unmanaged cloud resources
    …

CNAS-9: Inadequate ‘compute’ resource quota limits

Examples:

    Resource-unbound containers
    Over-permissive request quota set on APIs
    …

CNAS-10: Ineffective logging & monitoring (e.g. runtime activity)

Examples:

    No container or host process activity monitoring
    No network communications monitoring among microservices
    No resource consumption monitoring to ensure availability of critical resources
    Lack of monitoring on orchestration configuration propagation and stale configs
    …
