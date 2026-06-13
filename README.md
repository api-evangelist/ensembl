# Ensembl

Ensembl is a genome annotation database and browser maintained by the European Bioinformatics Institute (EMBL-EBI) and the Wellcome Sanger Institute. It provides comprehensive genome data for vertebrates and other eukaryotic organisms, covering gene annotation, variant data, regulatory features, comparative genomics, and evolutionary analysis across hundreds of species.

## REST API

The Ensembl REST API (v15.12) is available at https://rest.ensembl.org and provides language-agnostic HTTP access to Ensembl genome data without requiring local database installations. No authentication or API key is needed.

### Endpoint Categories

- **Archive** — Retrieve latest identifier versions
- **Comparative Genomics** — Gene trees, CAFE trees, alignments, homology
- **Cross References** — Map between Ensembl IDs and external databases
- **Information** — Species, assembly, biotype, and metadata queries
- **Linkage Disequilibrium** — LD calculations between variants
- **Lookup** — Identify species/database for genes and transcripts
- **Mapping** — Convert between coordinate systems and assemblies
- **Ontologies and Taxonomy** — Search term ancestry and relationships
- **Overlap** — Find overlapping genomic features by region
- **Phenotype Annotations** — Query phenotype-to-feature associations
- **Regulation** — Binding matrix retrieval
- **Sequence** — Genomic sequence retrieval with masking options
- **Transcript Haplotypes** — Phased haplotype computation
- **VEP** — Variant effect prediction (HGVS, IDs, regions)
- **Variation** — Variant queries by ID, PMID, or PMCID
- **Variation GA4GH** — GA4GH-standardized genomic data access

### Rate Limits

- 55,000 requests per hour per IP address
- Recommended self-throttle: 15 requests per second
- Rate limit headers: `X-RateLimit-Limit`, `X-RateLimit-Period`, `X-RateLimit-Remaining`, `X-RateLimit-Reset`
- HTTP 429 with `Retry-After` header when quota exceeded

## Resources

- [REST API Documentation](https://rest.ensembl.org/documentation)
- [Rate Limits Wiki](https://github.com/Ensembl/ensembl-rest/wiki/Rate-Limits)
- [GitHub Repository](https://github.com/Ensembl/ensembl-rest)
- [Jupyter Notebooks (Python/R)](https://github.com/Ensembl/rest-api-jupyter-course)
- [Terms of Use](https://www.ensembl.org/info/about/legal/index.html)
- [Privacy Notice](https://www.ebi.ac.uk/data-protection/ensembl/privacy-notice)
