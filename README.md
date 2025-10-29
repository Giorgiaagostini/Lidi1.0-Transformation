# 🧩 page2tei_mod

## Descrizione del progetto

Il presente repository contiene una versione modificata dello stylesheet XSL **`page2tei.xsl`**, denominata **`page2tei_mod`**, utilizzata per la trasformazione dei file XML esportati da **Transkribus** nel formato **TEI XML**.

Uno degli aspetti più delicati del flusso di lavoro è stato il passaggio da Transkribus al formato TEI, poiché — pur consentendo un’esportazione diretta — si è reso necessario garantire la **preservazione della marcatura personalizzata** e la **coerenza dei metadati**.

A tale scopo, è stata adottata e adattata la trasformazione **page2tei**, sviluppata da **Dario Kampkaspar**, realizzando una **versione modificata** specificamente pensata per le esigenze del progetto.

---

## ⚙️ Origine e finalità

**page2tei** è una trasformazione XSL che permette di convertire i file **PAGE XML** (prodotti da Transkribus) in **TEI XML**, offrendo maggiore flessibilità rispetto all’esportazione standard della piattaforma.

Le modifiche introdotte in **`page2tei_mod.xsl`** comprendono:

- Rimozione dei parametri e delle variabili non utilizzati o ridondanti  
- Personalizzazione del `<teiHeader>`  
- Ristrutturazione dell’elemento `<figure>`:  
  - sostituzione di `<head>` con `<ab>`  
  - aggiunta dell’elemento `<figDesc>` per una descrizione più completa  
- Gestione degli attributi `@ref` negli elementi `<persName>` e `<placeName>`

---

## 🔗 Riferimenti

- Dario Kampkaspar, *page2tei* — [GitHub Repository](https://github.com/dariok/page2tei)



