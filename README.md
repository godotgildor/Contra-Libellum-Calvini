# Contra Libellum Calvini — English Translation Project

An effort to produce an English translation of Sebastian Castellio's *Contra libellum Calvini* ("Against Calvin's Book"), written in 1554 as a response to John Calvin's defense of the execution of Michael Servetus. The work is a landmark text in the history of religious toleration and freedom of conscience.

## Project Overview

This repository documents the full pipeline from source manuscript to English translation:

1. **Source acquisition** — obtaining a scanned copy of the original Latin printing.
2. **OCR / text recognition** — converting the scanned images to machine-readable Latin text.
3. **Margin-text cleanup** — removing editorial marginalia so only the original manuscript text remains.
4. **Translation** — rendering the cleaned Latin into English (forthcoming).

## Source Manuscript

The original document was downloaded from the Princeton Theological Seminary digital collections:

- Source: https://commons.ptsem.edu/id/contralibellumca00cast
- Local copy: [`original_document/contralibellumca00cast.pdf`](original_document/contralibellumca00cast.pdf)

## OCR / Text Recognition

Text recognition was performed using [Transkribus](https://app.transkribus.org/).

- **Model:** *The Text Titan I ter* (released June 11, 2025)
- **About the model:** Text Titan I ter is a general-purpose Transkribus model for recognizing a wide variety of Latin scripts without custom training. It handles both printed and handwritten texts and performs well on historical documents, making it well suited to early modern printed works like this one.

## Margin-Text Cleanup

Many pages of the original printing include marginal annotations that are *not* part of Castellio's manuscript text — most often cross-references to source works and similar editorial notes. During OCR these marginal notes are frequently interleaved with the main text (sometimes inline within a line, sometimes segregated onto their own lines), as can be seen in the sample page below.

To recover the original manuscript text, each OCR'd page was reviewed manually and the identifiable margin text was removed, leaving (as closely as possible) only Castellio's own words.

### Sample Page

The image below illustrates the margin text problem — note the annotations running down the right-hand margin (e.g. *"Declaratio Calvini contra Serveti. Anno 1553…"*), which were removed during cleanup.

![Sample page from the original manuscript](original_document/sample_page.png)

## Status

- [x] Source manuscript acquired
- [x] OCR performed with Transkribus (Text Titan I ter)
- [x] Margin text removed from OCR output
- [ ] Cleaned Latin OCR text added to repository
- [ ] Translation prompt documented
- [ ] English translation completed and added to repository

## Roadmap

Future additions to this repository will include:

- A pointer to the final cleaned OCR Latin text.
- The LLM prompt used to perform the translation.
- A pointer to the completed English translation.

## About the Work

*Contra libellum Calvini* was written under the pseudonym Martinus Bellius (and circulated more widely after Castellio's death). It argues against the persecution and execution of those deemed heretics, responding directly to Calvin's *Defensio orthodoxae fidei* and its justification of Servetus's burning at Geneva in 1553. It stands alongside Castellio's *De haereticis, an sint persequendi* as a foundational document in the development of arguments for toleration and liberty of conscience.

## License

*(To be determined — consider noting the license for your translation and any methodology notes separately from the public-domain source text.)*
