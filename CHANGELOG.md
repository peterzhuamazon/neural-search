# CHANGELOG
All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). See the [CONTRIBUTING guide](./CONTRIBUTING.md#Changelog) for instructions on how to add changelog entries.

## [Unreleased 3.0](https://github.com/opensearch-project/neural-search/compare/2.x...HEAD)
### Features
### Enhancements
- Set neural-search plugin 3.0.0 baseline JDK version to JDK-2 ([#838](https://github.com/opensearch-project/neural-search/pull/838))
### Bug Fixes
- Fix for nested field missing sub embedding field in text embedding processor ([#913](https://github.com/opensearch-project/neural-search/pull/913))
### Infrastructure
### Documentation
### Maintenance
### Refactoring

## [Unreleased 2.x](https://github.com/opensearch-project/neural-search/compare/2.18...2.x)
### Features
- Pagination in Hybrid query ([#1048](https://github.com/opensearch-project/neural-search/pull/1048))
- Implement Reciprocal Rank Fusion score normalization/combination technique in hybrid query ([#874](https://github.com/opensearch-project/neural-search/pull/874))
### Enhancements
- Explainability in hybrid query ([#970](https://github.com/opensearch-project/neural-search/pull/970))
- Support new knn query parameter expand_nested ([#1013](https://github.com/opensearch-project/neural-search/pull/1013))
- Implement pruning for neural sparse ingestion pipeline and two phase search processor ([#988](https://github.com/opensearch-project/neural-search/pull/988))
- Support empty string for fields in text embedding processor ([#1041](https://github.com/opensearch-project/neural-search/pull/1041))
- Optimize ML inference connection retry logic ([#1054](https://github.com/opensearch-project/neural-search/pull/1054))
- Support for builder constructor in Neural Query Builder ([#1047](https://github.com/opensearch-project/neural-search/pull/1047))
- Validate Disjunction query to avoid having nested hybrid query ([#1127](https://github.com/opensearch-project/neural-search/pull/1127))
### Bug Fixes
- Address inconsistent scoring in hybrid query results ([#998](https://github.com/opensearch-project/neural-search/pull/998))
- Fix bug where ingested document has list of nested objects ([#1040](https://github.com/opensearch-project/neural-search/pull/1040))
- Fixed document source and score field mismatch in sorted hybrid queries ([#1043](https://github.com/opensearch-project/neural-search/pull/1043))
- Update NeuralQueryBuilder doEquals() and doHashCode() to cater the missing parameters information ([#1045](https://github.com/opensearch-project/neural-search/pull/1045)).
- Fix bug where embedding is missing when ingested document has "." in field name, and mismatches fieldMap config ([#1062](https://github.com/opensearch-project/neural-search/pull/1062))
- Fix explain exception in hybrid queries with partial subquery matches ([#1123](https://github.com/opensearch-project/neural-search/pull/1123))
- Handle pagination_depth when from =0 and removes default value of pagination_depth ([#1132](https://github.com/opensearch-project/neural-search/pull/1132))
- Fix single shard pagination issue of from ([#1140](https://github.com/opensearch-project/neural-search/pull/1140))
### Infrastructure
### Documentation
### Maintenance
- Add reindex integration tests for ingest processors ([#1075](https://github.com/opensearch-project/neural-search/pull/1075))
- Fix github CI by adding eclipse dependency in formatting.gradle ([#1079](https://github.com/opensearch-project/neural-search/pull/1079))
### Refactoring
