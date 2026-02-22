## About

### Vision

<!-- Understanding the human body and providing effective personalized healthcare is increasingly dependent
on our ability to process vast heterogeneous datasets. However, practitioners are often overwhelmed due to a lack
of tools and expertise in the field of data management. -->

This interdisciplinary workshop will focus on data management techniques, tools, and systems with direct
applications to the unique challenges in biomedical research and healthcare. Our goal is to build a lasting community
centered around these topics and spark fruitful collaborations.

> Biomedical research and healthcare are increasingly data-driven,
yet practitioners regularly struggle with data management challenges.

We are witnessing a proliferation of data collection technologies (e.g., electronic health records,
high-throughput sequencing, medical imaging), the growing adoption of computational methods for data analysis,
and the recognition that data is crucial for unlocking new scientific insights and improving patient
care. Furthermore, the scale of data that is being collected is growing exponentially,
driven by the decreasing costs of data acquisition technologies and the increasing digitization of healthcare systems.
However, the people who produce, analyze, and interpret biomedical data (e.g., clinicians, digital health
specialists, bioinformaticians, etc.) often lack the expertise and tools to effectively manage and analyze
these multi-modal datasets at scale. This means that scientific progress is often limited by overwhelming
data management challenges.

> Data management researchers are well-equipped to tackle many of these challenges, and are actively
seeking new research directions.

Data management researchers have spent decades developing techniques, tools, and systems for managing
large-scale data. They possess valuable expertise in areas such as data integration, data quality,
data governance, and scalable analytics. However, as evidenced by some points raised at panels at
SIGMOD and VLDB 2025, there is a growing push for data management researchers to actively pursue new,
high-impact application domains whose requirements can inspire fundamentally new system designs, benchmarks, and
end-to-end deployments. Biomedical data management is one such domain,
presenting unique research opportunities that can directly impact and improve human lives.

> Bringing these two communities together can unlock the potential for novel solutions and rapidly
accelerate scientific progress.

However, this is by no means a trivial task. One noteworthy challenge is that data management researchers often lack exposure to real-world biomedical
datasets (due to privacy restrictions), as well as the domain knowledge necessary to understand the specific
challenges and requirements of biomedical data management. Conversely, biomedical researchers often lack
awareness of the latest advances in data management research and how these techniques can be applied to their
specific problems. As a result, there is a gap between the capabilities of existing data management
systems and the needs of biomedical researchers and clinicians. Our goal is to bridge this gap
by bringing together experts from both communities to identify pressing biomedical data management challenges
and explore opportunities for collaboration that can lead to the development of novel data management
solutions tailored to the biomedical domain.

### Target audience

This workshop brings together two key groups, each one bringing a deep understanding of their own domain of
expertise and an interest in collaborating with the other side on projects that have the potential
to advance both fields:

* **Bioinformatics and Medical Informatics Experts:** Researchers and industry practitioners who understand specific
biomedical data domains (e.g., genomic data), the relevant questions that need to be asked, and the computational
steps that need to take place to answer those questions.

* **Data Management and Data Analysis Experts:** People with expertise in relevant subdomains of data management
(e.g., scalable analytics, data integration, data quality, streaming data management, etc.)
and large-scale data analysis, who have a desire or even a proven track record for making an impact
on the biomedical field.

### Motivating scenario

To provide an illustrative example of the kinds of challenges that this workshop aims to address, consider the
scenario of a [molecular tumor board (MTB)](https://en.wikipedia.org/wiki/Molecular_tumor_board).
It  is a multidisciplinary meeting in which experts from multiple disciplines
(e.g., oncologists, molecular biologists, pathologists, surgeons, genetic counselors) discuss a complex
patient case and converge on a treatment plan. Decisions must be made quickly, transparently, and with a
clear trail of supporting evidence. Such evidence is usually found by integrating highly multimodal evidence:
clinical data (diagnoses, medications, adverse events, patient history, and family),
high-throughput omics data (genome, transcriptome, proteome, genetic variations),
histopathological lab results, and tissue imaging, all of which are often originating from different institutions.

Given the number of patients, their uniqueness, and the time constraints of all the practitioners involved,
the board operates under tight time constraints and high stakes.
Time spent discussing a typical patient's case is measured in minutes,
while the preparation phase can take several hours of manual data preparation and analysis.

In practice, tumor board preparation often turns into an ad-hoc integration exercise across siloed systems and
heterogeneous formats. This setting exposes a set of recurring data management challenges:
data assembly across scales, statistical data quality assessments, integration across multiple external data sources,
intuitive data access, and scalability. A well-designed biomedical data management system could substantially reduce
these frictions, enabling a secure, patient-centric, multimodal view that is assembled reliably and quickly,
transforming tumor board preparation from a tedious, error-prone integration task into a reproducible workflow.

### Topics of interest

This workshop will feature presentations and discussions related to the following topics:

* **Domain-specific Data Models, and Interoperability** \
***Challenge:*** *Biomedical data spans many modalities with some existing standards, but interoperability remains bespoke and fragile.* \
***Related DM topics:*** [data modeling](https://en.wikipedia.org/wiki/Data_model), [data integration](https://en.wikipedia.org/wiki/Data_integration), [schema evolution](https://en.wikipedia.org/wiki/Schema_evolution) \
***Details:*** Interoperability between different standards across semantic and temporal scales, e.g.,
from ICU surveillance to patient histories and from single molecules to public health. This encompasses highly
heterogeneous data types, including raw genomic sequences, time series, omics measurements,
and high-content imaging, clinical records, biomedical knowledge graphs, and scientific publications.

* **Reproducible Data Preparation and Quality Control** \
***Challenge:*** *Biomedical analyses depend on complex, iterative data preparation and quality control steps that are rarely reproducible, auditable, or reusable.* \
***Related DM topics:*** [data lineage](https://en.wikipedia.org/wiki/Data_lineage), [data cleaning](https://en.wikipedia.org/wiki/Data_cleansing), [uncertain data models](https://en.wikipedia.org/wiki/Uncertain_data) \
***Details:*** Methods to ensure reproducibility and quality control of biomedical data processing and analysis despite regional,
temporal, and population-based differences.

* **Biomedical Analytics Pipelines and Platforms** \
***Challenge:*** *End-to-end biomedical analytics pipelines are difficult to scale, evolve, and reproduce using existing ad hoc workflow and data platform solutions.* \
***Related DM topics:*** [multi-modal data analytics](https://www.tiledb.com/multimodal-data), [materialized views](https://en.wikipedia.org/wiki/Materialized_view), [data indexing](https://en.wikipedia.org/wiki/Database_index) \
***Details:*** Optimization, scalability, and reusability of end-to-end analysis pipelines over large, heterogeneous,
streamed, and distributed biomedical data sets, possibly facing a variety of privacy regulations.
Knowledge graph construction and management for biomedical applications, including drug discovery and repurposing,
omics data analysis, and clinical decision-making.

* **Privacy, Governance, and Compliance** \
***Challenge:*** *Biomedical data must be analyzed under stringent privacy, governance, and regulatory constraints that complicate access and processing.* \
***Related DM topics:*** [access control](https://www.dataversity.net/articles/fundamentals-of-data-access-management/), policy-aware query execution, federated workload management \
***Details:*** Anonymization algorithms and procedures to ensure governance and regulation compliance for patient-related data. Systems for federated learning and privacy-preserving machine learning.

* **Human-centric and Organizational Challenges** \
***Challenge:*** *Deployments often fail because of mismatches between system design, user workflows, institutional incentives, and long-term maintenance realities.* \
***Related DM topics:*** human-in-the-loop data management, incentive-aware system design, data visualization \
***Details:*** Intuitive and powerful user interfaces and human-in-the-loop systems for biomedical practitioners.

### Specific goals

* **Introduction:** Exposure of data management experts to biomedical research questions, datasets, analytics pipelines, and domain-specific challenges. Conversely, exposure of bioinformatics experts to recent and advanced data management, data analysis, and data engineering techniques that can help overcome their challenges.
* **Scoping:** Identification of the most pressing challenges related to biomedical data management and analysis, having the biggest potential for fruitful synergistic efforts.
* **Collaboration:** Establishing lasting connections, determining modalities of collaboration, funding strategies, and publication venues.
* **Contribution:** Release of datasets, benchmarks, research project proposals, and a vision paper laying a foundation for future work in this space.
