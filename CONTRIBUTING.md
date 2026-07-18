# Contributing / 贡献指南

Thank you for helping maintain this collection. 欢迎补充恶意与钓鱼 URL 检测相关研究。

## Adding a paper / 新增论文

1. Add one row to the paper table in `README.md`.
2. Use the final published title and venue whenever available.
3. Link to a DOI or publisher page; an arXiv link may be added as a secondary resource.
4. Do not list a preprint and its final publication as separate papers.
5. If official code is available, add its GitHub repository in the GitHub column. Do not link unverified third-party implementations.
6. Use `—` when no official GitHub repository is available.

## Adding a dataset / 新增数据集

1. Add the dataset under the modality actually included in the released files: URL-only, webpage-derived features, visual/screenshot, or multimodal.
2. Link to the original publisher, institution, project page, or official repository. Avoid third-party mirrors when a primary source exists.
3. State the labels, approximate scale or update frequency, access method, and any registration or request requirement.
4. Distinguish raw HTML/screenshots from extracted webpage features. Do not describe a feature table as a raw webpage archive.
5. For live feeds, state that the source changes over time and encourage users to record the retrieval date and preserve a snapshot.
6. Confirm the source is publicly accessible for download, through an API/feed, or through a documented research-access request. Note applicable terms or licensing restrictions.

## Pull Request checklist

- [ ] The paper proposes, improves, or systematically studies malicious/phishing URL or webpage detection methods.
- [ ] Title, year, and venue match the publisher record.
- [ ] The entry is not a duplicate or an earlier version of an existing entry.
- [ ] DOI/publisher/arXiv links work.
- [ ] Any GitHub link is the official implementation or is clearly identified otherwise.
- [ ] The table remains sorted newest first.

For dataset contributions:

- [ ] The dataset directly supports malicious/phishing URL or webpage detection research.
- [ ] The modality category matches the released files.
- [ ] Labels, scale/update frequency, access conditions, and primary-source link are documented.
- [ ] Any license, Terms of Use, or research-only restriction is clearly noted.

## Corrections / 修正

Metadata and link corrections are encouraged. In the Pull Request description, link to the authoritative source supporting the change.
