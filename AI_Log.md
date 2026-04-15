# AI Log — CATENATE AI Academy

## 2026-04-09 — Giorno 1
- Task: Lettura documento INTRO (CATENATE AI Academy)
- Risultato: Completato. Concetti chiave assimilati: stack AI a livelli, deterministico vs non-deterministico, OWASP LLM Top 10, pattern architetturali in produzione, scala 7A.
- Tempo senza AI: n/a (lettura) | Tempo con AI: n/a
- Note: Livello 7A iniziale stimato A3-A4. Setup LM Studio avviato su MacBook Air M3 16GB con Gemma 3.

## 2026-04-10 — Giorno 2
- Task: Prima sessione AI — riepilogo documento CATENATE AI Academy Intro + esercizio L0 Giorno 1 (confronto 4 modelli + test autocontrollo) + esercizio L0 Giorno 2 (prompt engineering con 3 versioni su documento INTRO)
- Risultato: Prompt grezzo → output generico. Prompt raffinato → output preciso e strutturato. Confronto modelli: Gemini più verboso, ChatGPT più colloquiale, Claude più preciso sui limiti, Perplexity l'unico a cercare fonti. Sul test "sei sicuro?": Perplexity il più rigoroso, ChatGPT sycophantic, Gemini espansivo, Claude calibrato. Prompt few-shot → output più pulito e replicabile, seleziona i 4 concetti chiave giusti. Prompt strutturato → ha trovato affermazioni da verificare (statistica 985% McKinsey, $1B ARR Claude Code, break-even locale).
- Tempo senza AI: ~45 min (lettura) | Tempo con AI: ~45 min
- Note: Il prompt è l'interfaccia, non un optional. La reazione alla pressione rivela il carattere del modello più della risposta iniziale. Il few-shot è il migliore per analisi di documenti tecnici. Salvato Prompt Template 1 in prompt_templates.md.

## 2026-04-13 — Giorno 3, 4 e 5
- Task: Esercizio L0 Giorno 3 — classificazione e test di 3 task reali con AI + Esercizio L0 Giorno 4 — confronto 4 modelli (Claude, ChatGPT, Gemini, Perplexity) su task di riassunto documento Giorno 4 (Strumenti e Costi) + L0 Giorno 5 — Consolidamento + Quiz di autovalutazione (20 domande)
- Risultato:
  1. Rispondere a email → AI-assistito | Senza AI: 10 min | Con AI: 2 min | Risparmio: 8 min/email
  2. Riassumere documenti tecnici → AI-assistito | Senza AI: variabile | Con AI: pochi minuti | Risparmio: significativo su documenti lunghi
  3. Trascrivere e riassumere audio lezioni → AI-automatizzabile | Senza AI: 3 ore | Con AI: 5 min | Risparmio: ~175 min/lezione
  Confronto modelli su riassunto: tutti e quattro hanno risposto in modo istantaneo. Perplexity: prosa fluida con sintesi finale memorabile, cita fonti. Claude: il più sintetico, zero ridondanze. Gemini: bullet con titoli, aggiunge sezione esercizio pratico. ChatGPT: 10 bullet esatti, copertura totale, il più scansionabile. Quiz superato con successo. Settimana 1 (AI User) completata.
- Tempo senza AI: ~3h+ su task 3 | Tempo con AI: ~10 min totali (task mapping) + istantaneo per confronto modelli
- Note: Il task 3 è il moltiplicatore più alto in assoluto (36x). Il task 1 è il più immediato da integrare come micro-abitudine. Su task di riassunto strutturato le differenze tra modelli si appiattiscono rispetto al Giorno 1. Daily driver confermato: Claude per analisi approfondite, ChatGPT per riassunti veloci da condividere. Base solida su LLM, prompt engineering, strumenti e costi. 

## 2026-04-14 - Giorno 6 e 7
- Task: Esercizio L0 Giorno 6 - test RAG con NotebookLM su slide corso universitario Machine Learning (26 fonti PDF) + Esercizio L0 Giorno 7 - mappatura processo reale orchestrabile da un agente AI (pipeline studio)
- Risultato: 9 domande tecniche risposte correttamente con citazione delle slide specifiche. Domanda trappola (cosa NON è nelle slide): NotebookLM non ha inventato ma ha elencato gap e lacune del documento invece di ammettere un limite netto, comportamento ibrido, onesto ma non perfetto. Pipeline studio identificata come caso d'uso agente: registrazione lezione -> trascrizione (Whisper) -> riassunto (Claude) -> flashcard (Claude) -> salvataggio (Notion/NotebookLM). Human-in-the-loop dopo il riassunto, prima della generazione flashcard.
- Tempo senza AI: ~30 min (ricerca manuale nelle slide) + ~3h (pipeline studio manuale) | Tempo con AI: ~2 min (RAG) + ~10 min (pipeline automatizzata)
- Note: RAG funziona bene su domande dirette e ben documentate. Il limite emerge ai confini del corpus: il sistema ragiona sui gap invece di dire "non so". Il punto piu' fragile della pipeline studio e' la gestione del contesto su lezioni lunghe. Confermati i principi L0: un RAG mal fatto e' peggio di nessun RAG; chatbot risponde, agente risponde e agisce.
