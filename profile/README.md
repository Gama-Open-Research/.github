# Gama Open Research

<p align="center">
  <a href="https://github.com/Gama-Open-Research/.github/blob/main/profile/README.en.md"><img src="https://img.shields.io/badge/Read%20in-English-1f6feb?style=for-the-badge" alt="Read in English"></a>
  <a href="https://orcid.org/0009-0000-3113-9820"><img src="https://img.shields.io/badge/ORCID-0009--0000--3113--9820-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID"></a>
  <a href="https://www.linkedin.com/in/gabriel-gama-6301633b2/"><img src="https://img.shields.io/badge/LinkedIn-Gabriel%20Gama-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://zenodo.org/"><img src="https://img.shields.io/badge/DOI-Archived%20via%20Zenodo-024289?style=for-the-badge&logo=zenodo&logoColor=white" alt="Zenodo DOI"></a>
  <a href="https://www.go-fair.org/fair-principles/"><img src="https://img.shields.io/badge/Open%20Science-FAIR%20Principles-2ea44f?style=for-the-badge" alt="FAIR Principles"></a>
</p>

---

## Sobre a Organização

A **Gama Open Research** é a organização oficial destinada a armazenar, versionar e preservar as **pesquisas acadêmicas de [Gabriel Gama](https://orcid.org/0009-0000-3113-9820)**, reunindo em compêndios de pesquisa abertos (*Research Compendia*) todos os artefatos necessários para a **reprodutibilidade científica ponta a ponta**:

* **Artigos & Manuscritos Científicos (*Papers & Preprints*):** Códigos-fonte de artigos (R Markdown, LaTeX, BibTeX), tabelas automatizadas, figuras em alta resolução e materiais suplementares.
* **Bases de Dados & Evidências Empíricas (*Datasets*):** Conjuntos de dados brutos (`raw`) e processados/harmonizados (`processed`), dicionários de variáveis e fixtures de validação utilizados nos estudos.
* **Pipelines Analíticos & Experimentos (*Pipelines & Benchmarks*):** Scripts reprodutíveis de coleta, limpeza, resolução de entidades, modelagem estatística, matrizes de confusão e redes cienciométricas.
* **Notas Metodológicas & Cadernos de Pesquisa (*Research Notes*):** Protocolos experimentais, decisões de desenho de pesquisa, logs de auditoria de dados e documentação técnica para revisão por pares (*peer review*).

---

## Identificação Persistente via Zenodo (DOI) & Reprodutibilidade

> **Compromisso com a Rastreabilidade Científica:**
> **Quaisquer dados, pipelines e experimentos utilizados em publicação acadêmica apresentarão um identificador digital persistente (DOI) registrado via [Zenodo](https://zenodo.org/) (CERN) para fácil identificação, verificação independente e citação formal.**

Todos os repositórios vinculados a artigos publicados ou submetidos seguem os **[Princípios FAIR](https://www.go-fair.org/fair-principles/)** (*Findable, Accessible, Interoperable, Reusable*), garantindo que:
1. Cada versão exata dos dados e scripts utilizados em um artigo receba um **DOI único e imutável no Zenodo**;
2. Revisores, editores e pesquisadores possam auditar e reproduzir integralmente os resultados numéricos, tabelas e gráficos a partir do código-fonte;
3. Metadados de autoria e afiliação estejam padronizados via arquivos `CITATION.cff` e `.zenodo.json` vinculados ao ORCID do autor.

---

## Estrutura Padrão dos Repositórios de Pesquisa

Os compêndios de pesquisa dentro da **Gama Open Research** são organizados de forma modular para facilitar a auditoria e o reuso:

```text
paper-nome-do-estudo/
├── data/
│   ├── raw/                 # Dados brutos originais coletados nas fontes primárias
│   └── processed/           # Dados limpos, normalizados e prontos para análise (.csv / .RData)
├── pipeline/                # Scripts numerados de execução reprodutível (coleta, limpeza, análise)
├── notes/                   # Notas metodológicas, protocolos de pesquisa e diários de experimento
├── manuscript/              # Código-fonte do artigo (.Rmd / .tex) e referências (.bib)
├── output/                  # Tabelas, métricas de benchmark e figuras geradas automaticamente
├── CITATION.cff             # Metadados formais de citação do estudo
└── .zenodo.json             # Manifesto de indexação e registro de DOI no Zenodo
```

---

## Conheça também a BRAN Org (Brazilian Research Archive Network)

<p align="left">
  <a href="https://github.com/BRAN-Org"><img src="https://img.shields.io/badge/BRAN%20Org-Infraestrutura%20%26%20Ferramentas%20Abertas-6f42c1?style=for-the-badge&logo=github" alt="BRAN Org"></a>
  <a href="https://github.com/BRAN-Org/bibliolatam"><img src="https://img.shields.io/badge/R%20Package-bibliolatam-276DC3?style=for-the-badge&logo=r&logoColor=white" alt="bibliolatam"></a>
  <a href="https://doi.org/10.5281/zenodo.23623700"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.23623700.svg" alt="DOI bibliolatam"></a>
</p>

Enquanto a **Gama Open Research** concentra os repositórios de *papers*, experimentos, notas e dados de reprodutibilidade das pesquisas de Gabriel Gama, o desenvolvimento de **softwares científicos, pacotes R, APIs REST públicas e curadoria de bases históricas** acontece na **[BRAN Org (Brazilian Research Archive Network)](https://github.com/BRAN-Org)**.

A **[BRAN Org](https://github.com/BRAN-Org)** é uma iniciativa aberta de infraestrutura tecnológica e cienciométrica dedicada a resgatar, padronizar e preservar a produção científica brasileira e latino-americana. Entre seus principais projetos estão:

* **[`bibliolatam`](https://github.com/BRAN-Org/bibliolatam)** *(DOI: [`10.5281/zenodo.23623700`](https://doi.org/10.5281/zenodo.23623700))*: Pacote em R e aplicação web Shiny trilíngue (EN/PT/ES) para busca federada, reconstrução de redes de citação (JATS XML), normalização de autores regionais e fusão não-destrutiva de metadados das bases **SciELO, BDTD, Oasisbr, LA Referencia, Redalyc/AmeliCA e SPELL**, com total compatibilidade com o ecossistema `bibliometrix`.
* **Bases de Dados Bibliométricas Abertas & APIs REST:** Curadoria auditada e preservação digital de anais e acervos científicos nacionais, incluindo [`enancib-open-database`](https://github.com/BRAN-Org/enancib-open-database), [`ebbc-open-database`](https://github.com/BRAN-Org/ebbc-open-database), [`datagramazero-open-database`](https://github.com/BRAN-Org/datagramazero-open-database) e [`abec-open-database`](https://github.com/BRAN-Org/abec-open-database).

👉 **Visite e acompanhe a BRAN Org em: [https://github.com/BRAN-Org](https://github.com/BRAN-Org)**

---

## Pesquisador Responsável & Contato

* **Nome:** Gabriel Gama
* **ORCID:** [https://orcid.org/0009-0000-3113-9820](https://orcid.org/0009-0000-3113-9820) (`0009-0000-3113-9820`)
* **LinkedIn:** [https://www.linkedin.com/in/gabriel-gama-6301633b2/](https://www.linkedin.com/in/gabriel-gama-6301633b2/)
* **BRAN Org (Ferramentas & Infraestrutura):** [https://github.com/BRAN-Org](https://github.com/BRAN-Org)
* **GitHub Pessoal:** [https://github.com/GabrielBaiano](https://github.com/GabrielBaiano)
* **Portfólio & Website:** [https://gabrielbaiano.vercel.app/](https://gabrielbaiano.vercel.app/)
* **E-mail Acadêmico:** [gabrielngama@gmail.com](mailto:gabrielngama@gmail.com)
