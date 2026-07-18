# Awesome Malicious & Phishing URL Detection

[中文](#中文) | [English](#english)

A curated collection of high-quality detection research on malicious and phishing URLs and webpages.

## 中文

本仓库收录高水平的恶意 URL、钓鱼 URL 与钓鱼网页检测研究。收录论文应提出、改进或系统研究检测方法。欢迎通过 Pull Request 补充和修正。

### 论文

| Year | Paper | Journal / Conference | Paper Link | GitHub |
|---:|---|---|---|---|
| 2026 | IP-Augmented Multi-Modal Malicious URL Detection Via Token-Contrastive Representation Enhancement and Multi-Granularity Fusion | IEEE Transactions on Information Forensics and Security (TIFS) | [IEEE](https://ieeexplore.ieee.org/abstract/document/11592629/) · [arXiv](https://arxiv.org/abs/2510.12395) | [MACFormer](https://github.com/sevenolu7/MACFormer) |
| 2026 | URL2Graph++: Unified Semantic-Structural-Character Learning for Malicious URL Detection | Information Fusion | [DOI](https://doi.org/10.1016/j.inffus.2026.104209) · [arXiv](https://arxiv.org/abs/2509.10287) | — |
| 2026 | URL2Path: A Robust Graph Learning Approach for Malicious URL Detection | IEEE Transactions on Reliability | [IEEE](https://ieeexplore.ieee.org/document/11417329/) · [DOI](https://doi.org/10.1109/TR.2026.3668659) | — |
| 2025 | Continuous Multi-Task Pre-training for Malicious URL Detection and Webpage Classification | Computer Networks, 270: 111513 | [DOI](https://doi.org/10.1016/j.comnet.2025.111513) · [arXiv](https://arxiv.org/abs/2402.11495) | — |
| 2025 | From Past to Present: A Survey of Malicious URL Detection Techniques, Datasets and Code Repositories | Computer Science Review, 58: 100810 | [DOI](https://doi.org/10.1016/j.cosrev.2025.100810) · [arXiv](https://arxiv.org/abs/2504.16449) | [Open-source collection](https://github.com/sevenolu7/Malicious-URL-Detection-Open-Source) |
| 2025 | PMANet: Malicious URL Detection via Post-Trained Language Model Guided Multi-Level Feature Attention Network | Information Fusion, 113: 102638 | [DOI](https://doi.org/10.1016/j.inffus.2024.102638) · [arXiv](https://arxiv.org/abs/2311.12372) | [PMANet](https://github.com/Alixyvtte/Malicious-URL-Detection-PMANet) |
| 2025 | WebGuard++: Interpretable Malicious URL Detection via Bidirectional Fusion of HTML Subgraphs and Multi-Scale Convolutional BERT | arXiv | [arXiv](https://arxiv.org/abs/2506.19356) | — |
| 2025 | PhishAgent: A Robust Multimodal Agent for Phishing Webpage Detection | AAAI 2025 | [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/35003) · [arXiv](https://arxiv.org/abs/2408.10738) | — |
| 2024 | TransURL: Improving Malicious URL Detection with Multi-Layer Transformer Encoding and Multi-Scale Pyramid Features | Computer Networks, 253: 110707 | [DOI](https://doi.org/10.1016/j.comnet.2024.110707) · [arXiv / PyraTrans](https://arxiv.org/abs/2312.00508) | — |
| 2024 | KnowPhish: Large Language Models Meet Multimodal Knowledge Graphs for Enhancing Reference-Based Phishing Detection | USENIX Security 2024 | [USENIX](https://www.usenix.org/conference/usenixsecurity24/presentation/li-yuexin) · [arXiv](https://arxiv.org/abs/2403.02253) | [KnowPhish](https://github.com/imethanlee/KnowPhish) |
| 2024 | Less Defined Knowledge and More True Alarms: Reference-based Phishing Detection without a Pre-defined Reference List | USENIX Security 2024 | [USENIX](https://www.usenix.org/conference/usenixsecurity24/presentation/liu-ruofan) | [PhishLLM](https://github.com/code-philia/PhishLLM) |
| 2024 | PhishDecloaker: Detecting CAPTCHA-cloaked Phishing Websites via Hybrid Vision-based Interactive Models | USENIX Security 2024 | [USENIX](https://www.usenix.org/conference/usenixsecurity24/presentation/teoh) | [PhishDecloaker](https://github.com/code-philia/PhishDecloaker) |
| 2024 | VORTEX: Visual Phishing DetectiOns aRe Through EXplanations | ACM Transactions on Internet Technology, 24(2) | [DOI](https://doi.org/10.1145/3654665) | — |
| 2023 | A Large-Scale Pretrained Deep Model for Phishing URL Detection | IEEE ICASSP 2023 | [DOI](https://doi.org/10.1109/ICASSP49357.2023.10095719) | [FedURLBERT](https://github.com/Davidup1/FedURLBERT) |

### 去重说明

- `PyraTrans` 是 `TransURL` 的预印本名称，二者合并为一个条目。
- PMANet、URL2Graph++ 和 TIFS 论文的 arXiv 版本只作为资源链接，不重复计数。

### Public Datasets / 公开数据集

> [!IMPORTANT]
> 数据集按其**实际提供的模态**分类，而不是按论文所使用的全部特征分类。使用前请核对各数据源的许可、使用条款与采集时间；实时 feed 会持续变化，实验时应保存获取日期和数据快照。

#### URL-only / 纯 URL

| Dataset | Labels / Coverage | Scale / Update | Access | Notes |
|---|---|---|---|---|
| [ISCX-URL2016](https://www.unb.ca/cic/datasets/url-2016.html) | Benign, spam, phishing, malware, defacement | More than 114K URLs across five classes | Direct download | 适合多分类；由 UNB Canadian Institute for Cybersecurity 发布。 |
| [Phishing URL Dataset](https://data.mendeley.com/datasets/vfszbj9b36/1) | Phishing | 54,807 URLs | Direct download | 2024 年发布的静态钓鱼 URL 集。 |
| [PhishTank](https://www.phishtank.net/developer_info.php) | Community-verified phishing URLs with online status | Continuously updated | Feed / API | 开放社区 feed；应记录下载时间，并自行构造可信的良性对照集。 |
| [OpenPhish Community Feed](https://openphish.com/phishing_feeds.html) | Active phishing URLs | Updated every 12 hours; limited community feed | Direct feed | 免费社区版受其 Terms of Use 约束；学术实时数据与历史档案需另行申请。 |
| [URLhaus](https://urlhaus.abuse.ch/api/) | Malware-distribution URLs | Continuously updated | API / feeds | 面向恶意软件分发 URL，不等同于钓鱼数据；遵守 abuse.ch Fair Use Principles。 |

#### URL + Webpage-derived Features / URL＋网页衍生特征

| Dataset | Modalities / Features | Labels / Scale | Access | Notes |
|---|---|---|---|---|
| [PhiUSIIL](https://archive.ics.uci.edu/dataset/967/phiusiil%2Bphishing%2Burl%2Bdataset) | URL and corresponding webpage-derived attributes; 54 features | 235,795 labeled instances | Direct download | UCI 托管；提供提取后的特征，并非原始 HTML 网页归档。 |

#### Visual / Screenshot / 视觉截图

| Dataset | Modalities | Labels / Coverage | Access | Notes |
|---|---|---|---|---|
| [VisualPhish](https://s-abdelnabi.github.io/VisualPhishNet/) | Webpage screenshots | Trusted legitimate sites, targeted phishing pages, newly crawled phishing pages and benign sites | Request required | 仅限研究用途，按项目页面说明通过邮件申请。 |

#### Multimodal / 多模态

| Dataset | Modalities | Labels / Scale | Access | Notes |
|---|---|---|---|---|
| [Phishpedia Benchmark](https://github.com/lindsey98/Phishpedia) | URL, HTML, screenshot and target brand | 30K phishing webpages | Direct download | 官方仓库提供数据链接；适合视觉品牌识别与参考式钓鱼检测，不含良性类别。 |
| [TR-OP](https://github.com/imethanlee/KnowPhish#datasets) | Complete webpages for multimodal phishing evaluation | 5,000 benign + 5,000 phishing webpages | Direct download | KnowPhish 官方发布的平衡评测集；下载入口位于仓库的 Datasets 小节。 |

### 贡献

请阅读 [CONTRIBUTING.md](CONTRIBUTING.md)，通过 Pull Request 新增论文、公开数据集或修正元数据。论文应提供永久链接；数据集应提供官方来源、模态、标签/规模与访问条件。

## English

This repository curates high-quality detection research and public datasets for malicious and phishing URLs and webpages. Included papers should propose, improve, or systematically study detection methods. The tables above are the canonical paper and dataset lists.

Contributions are welcome. Please follow [CONTRIBUTING.md](CONTRIBUTING.md) and submit a Pull Request.

> [!NOTE]
> If this collection is helpful to your research, please consider citing our papers listed above.
>
> 如果本项目对您的研究有所帮助，欢迎引用我们在上方列出的相关论文。
