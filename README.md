# [Google Cloud Data Catalog][dc] - FAQ

> ⚠️ Beware: This is a **community-maintained** informal knowledge base.
>
> * Refer to the [**Data Catalog documentation**][docs] for the most up-to-date
>   information.

- **Is this repo useful?** Please **⭑Star** this repository and share the love.
- **Curious about something?** Open an [issue], someone may be able to add it to
  the FAQ.
- **Contribute** if you learned something interesting about Data Catalog.
- **Trouble using Data Catalog?** Ask a question [on Stack  Overflow][so].
  and tips.

[issue]: https://github.com/mesmacosta/datacatalog-faq/issues
[dc]: https://cloud.google.com/data-catalog
[ga]: https://cloud.google.com/blog/products/data-analytics/data-catalog-metadata-management-now-generally-available
[docs]: https://cloud.google.com/data-catalog/docs
[so]: https://stackoverflow.com/search?q=%5Bgoogle-cloud-platform%5D+data+catalog
[twitter]: https://twitter.com/mesmacosta
[search]: https://cloud.google.com/data-catalog/docs/how-to/search-reference
[quickstart-tagging]: https://cloud.google.com/data-catalog/docs/quickstart-tagging
[dlp-dc]: https://cloud.google.com/dlp/docs/sending-results-to-dc
[filesets]: https://cloud.google.com/data-catalog/docs/how-to/filesets
[medium - a mental model]: https://medium.com/google-cloud/data-catalog-hands-on-guide-a-mental-model-dae7f6dd49e
[medium - search and lookup]: https://medium.com/google-cloud/data-catalog-hands-on-guide-search-get-lookup-with-python-82d99bfb4056
[medium - templates and tags]: https://medium.com/google-cloud/data-catalog-hands-on-guide-templates-tags-with-python-c45eb93372ef
[medium - data governance]: https://towardsdatascience.com/boosting-the-data-governance-journey-with-google-cloud-data-catalog-d67acc3e3ffb
[medium - dc filesets]: https://medium.com/google-cloud/google-cloud-data-catalog-filesets-unlock-its-full-potential-5625c745303c
[tutorials - dlp to datacatalog tags]: https://cloud.google.com/community/tutorials/dlp-to-datacatalog-tags
[medium - looker integration]: https://medium.com/google-cloud/google-cloud-data-catalog-and-looker-integration-4ebefdef6a34
[medium - rdbms integration]: https://medium.com/google-cloud/google-cloud-data-catalog-integrate-your-on-prem-rdbms-metadata-468e0d8220fb
[medium - tableau integration]: https://medium.com/google-cloud/google-cloud-data-catalog-and-tableau-integration-204c1d17cc62
[medium - hive integration]: https://medium.com/@mesmacosta/google-cloud-data-catalog-keep-up-with-your-on-prem-hive-server-237edd1a1888
[medium - answer is data catalog]: https://medium.com/bluekiri/where-is-my-data-the-answer-is-google-data-catalog-acdbdf67eac6
[github - datacatalog connectors]: https://github.com/GoogleCloudPlatform/datacatalog-connectors
[github - datacatalog connectors bi]: https://github.com/GoogleCloudPlatform/datacatalog-connectors-bi
[github - datacatalog connectors hive]: https://github.com/GoogleCloudPlatform/datacatalog-connectors-hive
[github - datacatalog connectors rdbms]: https://github.com/GoogleCloudPlatform/datacatalog-connectors-rdbms
[github - templates_examples]: https://github.com/mesmacosta/datacatalog-util/blob/master/docs/templates_examples.md
-----

<!--
  ⚠️ DO NOT UPDATE THE TABLE OF CONTENTS MANUALLY ️️⚠️
  run `npx markdown-toc -i README.md`.

  Please stick to 80-character line wraps as much as you can.
-->

<!-- toc -->

- [Basics](#basics)
  * [What is Data Catalog?](#what-is-data-catalog)
  * [Is Data Catalog GA?](#is-data-catalog-ga)
  * [Is there a Mental Model for Data Catalog entities?](#is-there-a-mental-model-for-data-catalog-entities)
  * [How does Search Work?](#how-does-search-work)
  * [What are Templates and Tags for?](#what-are-templates-and-tags-for)
- [Open Source Connectors](#open-source-connectors)
  * [Can I ingest non-GCP assets into Data Catalog?](#can-i-ingest-non-gcp-assets-into-data-catalog)
  * [Can I ingest Looker assets into Data Catalog?](#can-i-ingest-looker-assets-into-data-catalog)
  * [Can I ingest Tableau assets into Data Catalog?](#can-i-ingest-tableau-assets-into-data-catalog)
  * [Can I ingest SQL Databases assets into Data Catalog?](#can-i-ingest-sql-databases-assets-into-data-catalog)
  * [Can I ingest Hive assets into Data Catalog?](#can-i-ingest-hive-assets-into-data-catalog)
- [Cloud Data Loss Prevention (DLP)](#cloud-data-loss-prevention-dlp)
  * [Does DLP has native support for Data Catalog?](#does-dlp-has-native-support-for-data-catalog)
  * [Can I run DLP in all my Big Query tables and send results to Data Catalog?](#can-i-run-dlp-in-all-my-big-query-tables-and-send-results-to-data-catalog)
- [Filesets](#filesets)
  * [What are use cases for Data Catalog Filesets?](#what-are-use-cases-for-data-catalog-filesets)
- [Samples](#samples)
  * [Do you have Templates examples to help me get started?](#do-you-have-templates-examples-to-help-me-get-started)
- [Other Community Articles](#other-community-articles)
  * [Is there a Data Governance overview with Data Catalog?](#is-there-a-data-governance-overview-with-data-catalog)
  * [Is there a blog post exploring the main features of Data Catalog?](#is-there-a-blog-post-exploring-the-main-features-of-data-catalog)

<!-- tocstop -->

-----

## Basics

### What is Data Catalog?

[Data Catalog][dc] Data Catalog is a fully managed and scalable metadata
management service that empowers organizations to quickly discover, understand,
and manage all their data. It offers a simple and easy-to-use search interface
for data discovery, a flexible and powerful cataloging system for capturing both
technical and business metadata, and a strong security and compliance foundation
with Cloud Data Loss Prevention (DLP) and Cloud Identity and Access Management (IAM) 
integrations.

### Is Data Catalog GA?
[Official Docs - GA blog post][ga] Yes, Data Catalog became GA, check the blog post.

### Is there a Mental Model for Data Catalog entities?
[Community - Data Catalog Mental Model][medium - a mental model] Yes, check this community blog post.

### How does Search Work?
[Official Docs - Search reference][search] Check the official docs for search syntax.

[Community - Data Catalog Search and lookup][medium - search and lookup] Check this community blog post for Python examples.

### What are Templates and Tags for?
[Official Docs - Quickstart Tagging][quickstart-tagging] Check the official docs for a quickstart on how to Tag Assets.

[Community - Data Catalog Templates and Tags][medium - templates and tags] Check this community blog post for Python examples.

## Open Source Connectors

### Can I ingest non-GCP assets into Data Catalog?
[Google Github - Datacatalog Connectors][github - datacatalog connectors] Yes, check the github repository for a list of open source connectors for non-GCP assets.

### Can I ingest Looker assets into Data Catalog?
[Google Github - Datacatalog Connectors BI][github - datacatalog connectors bi] Yes, check the github repository for sample code on how to ingest Looker assets.

[Community - Google Cloud Data Catalog and Looker integration][medium - looker integration] Check this community blog post, for an overview of the Looker integration.

### Can I ingest Tableau assets into Data Catalog?
[Google Github - Datacatalog Connectors BI][github - datacatalog connectors bi] Yes, check the github repository for sample code on how to ingest Tableau assets.

[Community - Google Cloud Data Catalog and Tableau integration][medium - tableau integration] Check this community blog post, for an overview of the Tableau integration.

### Can I ingest SQL Databases assets into Data Catalog?
[Google Github - Datacatalog Connectors RDBMS][github - datacatalog connectors rdbms] Yes, check the github repository for sample code on how to ingest RDBMS assets.

[Community - Google Cloud Data Catalog — Integrate Your On-Prem RDBMS Metadata][medium - rdbms integration] Check this community blog post, for an overview of the RDBMS integration.

### Can I ingest Hive assets into Data Catalog?
[Google Github - Datacatalog Connectors Hive][github - datacatalog connectors hive] Yes, check the github repository for sample code on how to ingest Hive assets.

[Community - Google Cloud Data Catalog — Keep Up With Your On-Prem Hive Server][medium - hive integration] Check this community blog post, for an overview of the Hive integration.

## Cloud Data Loss Prevention (DLP)

### Does DLP has native support for Data Catalog?
[Official Docs - Sending Cloud DLP scan results to Data Catalog][dlp-dc] Check the official docs for instructions.

### Can I run DLP in all my Big Query tables and send results to Data Catalog?
[Community - Create Data Catalog tags by inspecting BigQuery data with Cloud Data Loss Prevention][tutorials - dlp to datacatalog tags] check this community tutorial for instructions.

## Filesets

### What are use cases for Data Catalog Filesets?
[Official Docs - Using Cloud Storage filesets][filesets] Check the official docs.

[Community - Google Cloud Data Catalog Filesets: unlock its full potential][medium - dc filesets] Check this community blog post, if you want to enrich your filesets with Tags containing stats about your cloud storage files.

## Samples

### Do you have Templates examples to help me get started?
[Community - Data Catalog Template examples][github - templates_examples] Check this community github, if you are looking for guidance on what fields use on your Templates. There's an option to create the sample Templates in your Project using `datacatalog-util` Python package.

## Other Community Articles

### Is there a Data Governance overview with Data Catalog?
[Community - Boosting the Data Governance journey with Google Cloud Data Catalog][medium - data governance] Check this for a Data Governance and Data Catalog community blog post.

### Is there a blog post exploring the main features of Data Catalog?
[Community - Where is my data? The answer is Google Data Catalog][medium - answer is data catalog] Check this for a blog post exploring the main features of Data Catalog.

> **Your question not answered here?** Open an [issue] and see if we can answer.
