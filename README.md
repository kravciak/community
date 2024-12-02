# A Year in Review: Kubewarden's Progress in 2024

2024 was a milestone year for Kubewarden, filled with exciting advancements, impactful releases, and growing community engagement. Across performance improvements, enhanced features, and innovative policies, Kubewarden continued to redefine Kubernetes policy management. Let’s explore the highlights of this remarkable year.

## Streamlined Performance and Improved Reliability

The year began with the release of **Kubewarden 1.10**, which introduced substantial optimizations for policy server performance. Memory usage was streamlined, enabling constant consumption even in large deployments. These improvements, powered by smarter Wasmtime pre-initialization, eliminated memory leaks and enhanced reliability. Policy evaluation now operates on-demand, ensuring a fresh, clean state for every request.

Meanwhile, Go developers gained the ability to create context-aware policies with Kubernetes resource insights. This addition expanded Kubewarden’s flexibility, allowing WASI policies to take full advantage of Kubernetes capabilities. These features laid the groundwork for continued performance-focused updates.

## Scaling for Complexity and Security

With **Kubewarden 1.11**, the focus shifted to scaling for large and complex Kubernetes clusters. The Audit Scanner saw significant enhancements, including parallelized operations, reducing resource consumption and improving efficiency. New host capabilities allowed policies to retrieve OCI image manifests, empowering developers to enforce stricter security standards by inspecting container configurations in detail.

The momentum carried into **1.12 and 1.13**, which emphasized high availability and better resource management. PolicyServer deployments gained support for PodDisruptionBudgets, affinity rules, and resource limits, ensuring stability in production environments. Gatekeeper policies saw a 55% performance boost, and memory usage was dramatically reduced for clusters managing thousands of resources. These updates reinforced Kubewarden’s commitment to scalability and efficiency.

## Unlocking New Possibilities with CEL and Policy Groups

Mid-year, Kubewarden introduced groundbreaking innovations. The **CEL policy**, launched with **1.14**, provided a new DSL for policy writing, leveraging the Common Expression Language. This feature was backward-compatible with Kubernetes’ ValidatingAdmissionPolicies and expanded functionality by integrating Kubewarden’s host capabilities.

Shortly after, the **Policy Groups** feature arrived in **1.17**, allowing users to combine multiple policies with logical expressions. These groups reduced complexity while enabling advanced validations, like ensuring unique Kubernetes service selectors or enforcing organizational rules. This innovation marked a significant leap forward, enabling users to create powerful, reusable policies with ease.

## Enhanced Security and Sustainability

By the time **Kubewarden 1.17** was released, the project had automated certificate generation and rotation, removing the dependency on cert-manager. This self-sufficient approach ensured seamless management of TLS certificates, simplifying operations while enhancing security. The subsequent **1.18** release brought even greater assurance with the project achieving **SLSA Level 3 compliance**, a critical milestone in supply chain security.

## Growing Community and Ecosystem

Beyond technical achievements, 2024 saw significant efforts to strengthen the Kubewarden community. A new [community repository](https://github.com/kubewarden/community) was launched to consolidate documentation, guidelines, and contributor resources. This initiative made it easier for new and experienced contributors to engage with the project.

Kubewarden also expanded its policy library, refining existing policies like `verify-image-signatures` and `trusted-repos` to support all Kubernetes workloads. Meanwhile, its growing presence at KubeCon events and partnerships, such as tutorials in Rancher Academy, underscored its leadership in Kubernetes policy management.

## Looking Ahead

As the year concludes, Kubewarden is poised for even greater innovation in 2025. Plans include extending the capabilities of Policy Groups, refining certificate management, and introducing developer-focused tools for automation and testing. These initiatives promise to make Kubernetes policy management even more accessible and powerful.

To our community, thank you for making 2024 such a memorable year. Your contributions, feedback, and enthusiasm drive Kubewarden’s success. Let’s continue shaping the future of Kubernetes security together. 

Join the conversation on [Slack](https://kubernetes.slack.com/?redir=%2Fmessages%2Fkubewarden) or participate in our [community meetings](https://teamup.com/ks2bj74dvw132mhjtj). Here’s to another year of innovation and collaboration. 

Happy policy writing!
