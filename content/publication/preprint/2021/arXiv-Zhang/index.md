---
title: "A lightweight blockchain-based access control scheme for integrated edge computing in the internet of things"
authors:
- Jie Zhang
- admin
- Lingyun Yuan

date: "2021-11-17T00:00:00Z"
doi: "10.48550/arXiv.2111.06544"

# Schedule page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: "arXiv:2111.06544"
publication_short: ""

abstract: In view of the security issues of the Internet of Things (IoT), considered better combining edge computing and blockchain with the IoT, integrating attribute-based encryption (ABE) and attribute-based access control (ABAC) models with attributes as the entry point, an attribute-based encryption and access control scheme (ABE-ACS) has been proposed. Facing Edge-Iot, which is a heterogeneous network composed of most resource-limited IoT devices and some nodes with higher computing power. For the problems of high resource consumption and difficult deployment of existing blockchain platforms, we design a lightweight blockchain (LBC) with improvement of the proof-of-work consensus. For the access control policies, the threshold tree and LSSS are used for conversion and assignment, stored in the blockchain to protect the privacy of the policy. For device and data, six smart contracts are designed to realize the ABAC and penalty mechanism, with which ABE is outsourced to edge nodes for privacy and integrity. Thus, our scheme realizing Edge-Iot privacy protection, data and device controlled access. The security analysis shows that the proposed scheme is secure and the experimental results show that our LBC has higher throughput and lower resources consumption, the cost of encryption and decryption of our scheme is desirable.

# Summary. An optional shortened abstract.
summary: Lightweight blockchain, Edge Computing, Internet of thinges, Access control, Attribute-based encryption, Security.

tags: 
- IoT
- Blockchain
- ABAC
- edge computing
- ABE
featured: false

links:
- name: Arxiv
  url: https://arxiv.org/abs/2111.06544
url_pdf: https://jackaugust.github.io/files/2111.06544.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'The four-layer structural framework followed in our scheme.'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

This paper is about data security in Edge-Iot. To accomplish lightweight encryption outsourcing in an edge-device architecture, improved CP-ABE algorithm. Then to achieve the secure access to IoT data, attempt have been made to implement an attribute-based access control model. Try to build a blockchain network on a restricted terminal, built a lightweight blockchain LBC to adapt to IoT.

> Give a specific comparison:

1. Comparison of theoretical overhead with other papers on CP-ABE’s outsourced computation;
2. Comparing the cost of lightweight blockchain LBC with private Fabric and Ethereum;
3. Give the implementation algorithm of access control related contracts;


> Why not Submit:

1. The biggest problem is that the scene is not clear, the research value is not sufficient;
2. Then the security proof is weak, the research content is not specific enough;
3. The security strength between access control and ciphertext is repeated

Zhang J, Yuan L, Xu S. *A lightweight blockchain-based access control scheme for integrated edge computing in the Internet of Things*[J]. arXiv preprint arXiv:2111.06544, 2021.
