# Generatore Open Day — Med & Tech

Tool web statico per generare nomenclatura BM (Campagna · Ad Set · Creatività) + copy creative + paragrafo modulo Lead Ads per le campagne **Open Day Total Lift** e **Open Day Total Sculpt** del cliente **Med & Tech**, gestite da [FMM Consulting](https://fmmconsulting.it).

## Online

👉 **<https://advfmosca.github.io/generatore-open-day-medtech/>**

Apri il link da qualunque browser (anche mobile). Nessun login richiesto.

## Cosa fa

1. Selezioni il **front-end**: Total Lift oppure Total Sculpt.
2. Inserisci i dati dell'evento: nome farmacia/studio, nome dottoressa (BM + copy), data evento, indirizzo.
3. Il tool calcola automaticamente:
   - nome campagna in nomenclatura FMM (`Open Day - Total Lift - {NOME_DOTTORESSA}`)
   - nome ad set con date precise (`PUBBLICO FREDDO - {COGNOME} | Dal {gg.mm} al {gg.mm}`) — date dell'ad set = evento − 14gg → evento − 1gg
   - nome creatività (`{gg-mm-aaaa}`)
   - 3 variant di copy Facebook/Instagram da incollare nelle creatività
   - paragrafo descrittivo del modulo Lead Ads
   - link al template Canva del video creativo

## Convenzione di naming (essenziale per i report)

Le automazioni di reporting (Windsor.ai → Slack `#cea-medandtech-b2c`, daily check, scheduled tasks) si basano sulla nomenclatura BM rigida generata da questo tool. **Nomi sbagliati = dati sbagliati nei report.** Usare sempre il generatore, mai scrivere a mano.

## Note tecniche

- File HTML self-contained: nessuna dipendenza CDN, nessun backend, nessun cookie/storage. Renderizza ovunque.
- Ultima modifica copy Total Sculpt: **12/05/2026** — nuova narrativa unica in rotazione (niente A/B testing su Sculpt). Cronologia delle modifiche: vedi log del repo.
- Sorgente: questo repository (`index.html`).

## Repository correlati

- [`advfmosca/med-tech-daily-check`](https://github.com/advfmosca/med-tech-daily-check) — pipeline daily check campagne Open Day attive.

---

© FMM Consulting di Francesco Maria Mosca · P.IVA IT06071370651
