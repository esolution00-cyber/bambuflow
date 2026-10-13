# BambuFlow by e-solution

**Public technical preview · R12.7.2**

[Open the public preview](https://bambuflow.esolution.it/) · [e-solution](https://www.esolution.it/)

BambuFlow is an e-solution project for preparing Bambu-oriented 3MF workflows in a clear, traceable and evidence-driven way. It helps separate what is contained in a file, what is declared by the operator, and what still needs to be verified in Bambu Studio, on the selected machine or through a physical test.

The current public release is a **technical preview**, not a finished optimization service and not an official Bambu Lab product.

## One environment, several dedicated surfaces

BambuFlow is part of a wider e-solution system rather than a standalone landing page. Different connected interfaces address different stages of the same Bambu-oriented journey:

- finding or selecting a model;
- configuring a product, material and colour;
- scaling, subdividing and preparing joints for oversized geometry;
- obtaining a quotation and moving toward a controlled purchase;
- checking the 3MF and documenting the path through Bambu Studio Preview;
- preserving evidence for later production and quality review.

This separation keeps each task understandable while the complete environment follows one validation method and one public/private boundary.

## Bambu-first direction

The current engineering and validation effort is intentionally **Bambu-first**. We are building depth around Bambu Studio, Bambu Lab machines and their real production workflow instead of presenting a superficial generic multi-brand wrapper.

Our preferred long-term direction is to mature the system through a direct technical relationship with Bambu Lab. The architecture remains modular and evidence-based, so additional manufacturers could be supported in the future without weakening or rewriting the Bambu work already validated. No exclusivity or formal relationship is claimed at the current stage.

## What can be tested today

- local inspection of a selected 3MF file in the browser;
- defensive checks on the ZIP/3MF container before reading its structure;
- recognition of core 3MF parts and available Bambu metadata;
- explicit detection of the source-machine identity and source/target mismatches;
- guided configuration for the e-solution Bambu Lab H2S and H2C workflow;
- controlled conversion of compatible Bambu-origin projects to resolved official H2S or H2C machine, process and filament identities;
- removal of source slicing artefacts before the converted candidate is downloaded, so an old machine's G-code cannot be carried into the new project;
- structural validation of ScalaForge-generated 3MF hand-offs and the Bambu Studio project envelope before candidate generation;
- selection of one or more priorities, including quality, strength, speed, finish and precision;
- a synthetic ScalaForge/H2S hand-off fixture with 10/10 browser preflight checks;
- a separate hand-off checklist for Bambu Studio Preview;
- export of a reproducible JSON dossier after the required gates are complete.

For the R12.7.2 synthetic ScalaForge/H2S fixture, candidate generation, browser download and 3MF integrity were verified. Bambu Studio Preview was verified separately on the canonical equivalent, not on the downloaded public artifact. This demonstrates the hand-off workflow only; it does not establish optimization or physical quality, fit, strength or finish.

The selected file remains in the browser during the public preflight. A converted candidate preserves the model geometry and must be sliced again and inspected in Bambu Studio Preview. The public interface does not start a printer, send G-code, modify a machine, or silently change an installed preset.

## What is still under development

- measurable optimization candidates beyond the current machine-profile conversion;
- same-version slicing of original and candidate;
- comparative G-code evidence for time, material, layers, supports, pauses, tool changes and Z height;
- automatic rejection of candidates without a measurable advantage;
- controlled GitHub Issues integration through a future GitHub App;
- wider validation across real, anonymized projects.

Until these gates are complete, BambuFlow does **not** describe its generated files as optimized production files.

## Validation model

```text
e-solution experience
        ↓
official manuals and compatible profiles
        ↓
comparable slicing and G-code evidence
        ↓
Bambu Studio Preview
        ↓
physical sample or complete-part validation
        ↓
separate human authorization to print
```

Each stage answers a different question. A valid archive is not proof of printability; successful slicing is not proof of dimensional fit, strength or finish; a preview is not authorization to start a machine.

## Public ecosystem

- [BambuFlow](https://bambuflow.esolution.it/) — 3MF preflight and documented validation path;
- [Stampa 3D](https://www.esolution.it/stampa-3d-su-richiesta/) — model configuration, quotation and controlled purchase workflow;
- [ScalaForge 3D](https://www.esolution.it/scalaforge-3d/) — large-format scaling, subdivision, joints and tolerance preparation;
- [Prodotti 3D](https://www.esolution.it/prodotti-3d/) — configurable e-solution 3D-printed products.

These are separate user interfaces within one connected environment, not unrelated projects.

## GitHub integration direction

The planned integration uses a GitHub App with the smallest practical scope:

- access only to repositories explicitly selected by the user;
- initial permissions limited to the Issues workflow;
- no access to local project files, printer credentials or unrelated repositories;
- issue creation only after an explicit user action;
- no publication of customer files or private production evidence.

The GitHub App has not yet been registered. Callback URLs, webhooks and permissions will be declared only after the corresponding endpoints and public policies exist and have been tested.

## Public/private boundary

This repository is a public presentation and progress record. It does not distribute the private optimization engine, customer archives, production presets, VPS configuration, credentials or the complete e-solution decision system.

No license is granted to reuse the BambuFlow or e-solution names, visual identity or proprietary workflow. Code or assets explicitly released in the future will carry their own license.

## Status and feedback

Current public revision: **R12.7.2 technical preview**

Primary URL: [https://bambuflow.esolution.it/](https://bambuflow.esolution.it/)

Technical feedback may be submitted through this repository after the public issue templates are activated. Commercial or production enquiries should use the official [e-solution website](https://www.esolution.it/).

## Trademark notice

Bambu Lab, Bambu Studio and the names of Bambu Lab products are trademarks of their respective owner. BambuFlow is an independent e-solution project and is not currently sponsored, endorsed or affiliated with Bambu Lab.

---

## Sintesi in italiano

BambuFlow è un progetto indipendente di e-solution per controllare file 3MF, definire priorità di ottimizzazione e preparare un percorso di verifica riproducibile attraverso Bambu Studio Preview. La versione pubblica R12.7.2 aggiunge il controllo strutturale del passaggio 3MF generato da ScalaForge e dell'involucro di progetto riconosciuto da Bambu Studio. Una fixture sintetica con destinazione H2S ha superato 10/10 controlli di preflight; generazione, download e integrità dell'archivio sono stati verificati. La Preview nativa è stata controllata separatamente sulla candidata canonica equivalente, non sul file scaricato dal flusso pubblico. È una verifica del flusso software, non una prova di ottimizzazione o qualità fisica. BambuFlow resta un'anteprima tecnica: non controlla la stampante, non avvia stampe e non dichiara le candidate come file di produzione ottimizzati.

Il metodo mantiene distinti preflight del file, slicing comparabile, lettura del G-code, Preview, prova fisica e autorizzazione alla stampa.

BambuFlow, Stampa 3D, ScalaForge 3D e Prodotti 3D sono pagine specializzate di un unico ambiente e-solution oggi sviluppato in profondità attorno al flusso Bambu Lab. L'obiettivo preferenziale è maturarlo attraverso un rapporto tecnico diretto con Bambu Lab; l'architettura resta modulare e potrà supportare in futuro altri produttori senza disperdere il lavoro Bambu già validato. Allo stato attuale non viene dichiarato alcun rapporto formale o di esclusiva.
