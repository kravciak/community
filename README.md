# A Year in Review: Kubewarden's Progress in 2024

2024 has been a transformative year for the Kubewarden project, marked by significant releases, exciting innovations, and growing community engagement. Here's a look back at the major milestones and advancements that defined the year.

## Key Releases and Features

### Kubewarden 1.10: Performance and Reliability Upgrades
The year began with **Kubewarden 1.10**, focusing on optimizing performance:
- **Reduced memory usage**: Policy servers now exhibit constant memory consumption regardless of scaling, thanks to Wasmtime's pre-initialization and deduplication of policy evaluators.
- **Context-aware WASI policies in Go**: Go developers can now write policies leveraging Kubernetes resource context.
- **Controller and Audit Scanner enhancements**: Strengthened defenses against policy webhook modifications and added an in-memory store for audit results.

### Kubewarden 1.11: Scaling for Larger Clusters
The release emphasized **audit efficiency and host capabilities**:
- Audit Scanner's parallelized operations significantly reduced time and memory usage.
- A new capability to retrieve OCI manifests allowed policies to inspect container configurations, empowering deeper policy validations.

### Kubewarden 1.12 and 1.13: High Availability and Enhanced Scalability
These versions introduced:
- **PolicyServer HA features**: Configuration for PodDisruptionBudgets, resource limits, and affinity rules.
- **Performance boosts for Gatekeeper and context-aware policies**: A 55% improvement for Gatekeeper policies and memory savings for large-scale Kubernetes clusters.
- **Policy updates**: Expanded the `verify-image-signatures` and `trusted-repos` policies, enhancing flexibility and compliance.

### Kubewarden 1.14 to 1.16: Evolution in Policy Writing
The project focused on simplifying policy development:
- **CEL policy**: A versatile policy supporting Kubernetes ValidatingAdmissionPolicies with Kubewarden-specific extensions.
- **Policy groups**: Introduced in 1.17, enabling compound policies to combine existing ones using logical expressions, offering users a powerful, modular approach to policy management.

### Kubewarden 1.17 and 1.18: Maturity and Security
The later releases showcased:
- **Certificate rotation automation**: Eliminated reliance on cert-manager, introducing a seamless mechanism for managing TLS certificates.
- **SLSA Level 3 compliance**: Achieved higher supply chain security standards, reflecting Kubewarden's commitment to trust and reliability.

## Community and Ecosystem Growth

### New Community Repository
In response to CNCF recommendations, a new [community repository](https://github.com/kubewarden/community) consolidates documentation and resources. This initiative fosters transparency and eases onboarding for contributors.

### Policy Expansion
2024 saw the release and updates of key policies:
- **Environment Variable Policy**: Enhanced to validate variable names independently.
- **Trusted Repos Policy**: Fully rewritten to support all Kubernetes workloads.

### Engagement Highlights
- **KubeCon EU and NA**: The team showcased Kubewarden’s capabilities, receiving enthusiastic feedback.
- **Rancher Academy**: Tutorials featured Kubewarden, underlining its adoption in cloud-native security education.

## Looking Ahead

Kubewarden is set to explore further innovations, including:
- **PolicyGroup enhancements**: Expanding support for complex policy compositions.
- **Certificate management refinements**: Streamlining integration with Kubernetes clusters.
- **Automation and developer tooling**: Continuing efforts in Helm chart testing and CI/CD optimizations.

## A Final Note of Gratitude

To our community, thank you for contributing to Kubewarden’s journey. Your input, whether in Slack discussions, GitHub contributions, or through direct feedback, has been invaluable.

As we look toward 2025, we invite everyone to stay connected through our [Slack channel](https://kubernetes.slack.com/?redir=%2Fmessages%2Fkubewarden) and [community meetings](https://teamup.com/ks2bj74dvw132mhjtj). Together, let’s continue shaping the future of Kubernetes policy management.

Happy policy writing!
