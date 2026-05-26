# Proposal to create the vdb-streambench Repository

## Basic Project Information

Project Name: vdb-streambench

Project Purpose:

vdb-streambench is a reproducible streaming-ingestion benchmark tool across multiple vector databases, built on VectorDBBench's StreamingPerformanceCase. It evaluates how each database performs while data is continuously being inserted — balancing index construction, write throughput, search latency, recall, and memory usage under a realistic production pattern.

Value in the OceanBase open source ecosystem:

- Aligned with **SIG AI**'s direction of "Database and AI mutual empowerment," providing a standardized streaming performance evaluation platform for the vector database ecosystem.
- Supports SeekDB, Milvus, Elasticsearch, Chroma, Qdrant, and LanceDB, covering a wide range of vector database use cases.
- Supports both local and remote (split client/server) deployment modes, suitable for diverse testing environments.
- Provides reproducible benchmark reports to assist users in vector database selection and comparison.

Repository URL: <https://github.com/oceanbase/vdb-streambench>

Project Owner (GitHub ID):

- Maintainer: liuhao6741

> Additional Maintainers / Committers may be added during the review process.

License: Apache 2.0 (consistent with the prevailing OceanBase community license)

## Open Source Project Checklist

> The checklist is intended to make the project more standardized and easier for community users to use. The items in the checklist should be completed as soon as possible after the project is created.

- [x] Includes README.md
- [ ] Engineering projects should include CONTRIBUTING.md. Refer to the OceanBase community [CONTRIBUTING file](https://github.com/oceanbase/.github/blob/main/CONTRIBUTING.md)
- [ ] Includes CODE_OF_CONDUCT.md (if not present, the existing community [Code of Conduct](https://github.com/oceanbase/.github/blob/main/CODE_OF_CONDUCT.md) will be used)
- [x] Engineering projects include user installation instructions (typically in README.md)
- [x] Engineering projects include user usage instructions (typically in README.md)
- [ ] Engineering/code projects include build instructions (typically in README.md)

## Voting Deadline

If the voting conditions are not met, this vote will close on **June 9, 2026**.

> Voting conditions are met when the vote has succeeded (e.g., at least 2/3 of TOC members have voted in favor) or failed (e.g., half of TOC members have voted against).

## Voting Results

Refer to [vdb-streambench project creation vote result](a pull request link).
