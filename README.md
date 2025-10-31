[README_Hotel5L_Analisi_FnB.md](https://github.com/user-attachments/files/23277452/README_Hotel5L_Analisi_FnB.md)# 🏨 Hotel 5★ Lusso – Analisi Strategica Food & Beverage e Controllo di Gestione
**Autore:** Riccardo Avitabile  
**Strumento:** Power BI Desktop  
**Versione modello:** Hotel5L_Analisi_FnB_Template.pbit  

---

## 🎯 Obiettivo del progetto
Questo progetto Power BI nasce per supportare l’analisi direzionale e il controllo di gestione negli **hotel 5 stelle lusso**, con un focus specifico su:

- Performance economiche complessive (ADR, RevPAR, TRevPAR, GOP, Food Cost %)
- Analisi dei costi **Food & Beverage**
- Monitoraggio di **Complimentary e Attese Camera**
- Simulazioni predittive What-If su prezzi, costi e marginalità

---

## 📊 Struttura del modello

| Pagina | Descrizione |
|:-------|:-------------|
| **README** | Guida alla navigazione e legenda KPI |
| **Executive** | Cruscotto direzionale con indicatori chiave (ADR, RevPAR, GOP, Food Cost %) |
| **F&B & Costing** | Analisi Food & Beverage, Complimentary e costi operativi |
| **Scenario (What-If)** | Simulatore di scenario per prezzo camere, food cost e complimentary |

---

## 📂 Dataset inclusi
Tutti i dati sono caricati da fonti Excel simulate con struttura coerente a quella di un sistema PMS reale:

- `hotel5L_reali_template_budgeted.xlsx`  
- `f_capacita_camere.xlsx`  
- `f_budget.xlsx`  
- `scenario_params.xlsx`  

Le tabelle sono organizzate per **modello a stella** (dimensioni + fatti) e relazionate tramite **Power Query e PowerPivot**.

---

## ⚙️ Misure principali (DAX)
Alcune delle misure chiave usate nel modello:

```DAX
Food Cost % = DIVIDE([Costo F&B (Materie Prime)], [Ricavi F&B])
GOP = [Ricavi Totali] - [Costi Operativi]
GOP% = DIVIDE([GOP], [Ricavi Totali])
GOPPAR = DIVIDE([GOP], [RoomNights Disponibili])
```

> Sono inclusi anche semafori colore (verde/giallo/rosso) per Food Cost % e GOP%, oltre a misure “Potenziale” e “Scenario What-If”.

---

## 🎨 Layout e Tema
Il modello utilizza un **tema blu-oro** con tre layout coordinati:

- `powerbi_page_bg_executive.png`
- `powerbi_page_bg_fnb_costing.png`
- `powerbi_page_bg_scenario.png`

---

## 🚀 Come aprire il progetto
1. Estrai tutti i file nella cartella  
   `C:\Users\riccardo\Downloads\Hotel5L_Analisi_FnB\`
2. Apri il file  
   `Hotel5L_Analisi_FnB_Template.pbit`  
3. Power BI creerà automaticamente il file `.pbix` con tutti i dati e dashboard operative.

---

## 📈 Risultati e insight
- **Riduzione del Food Cost %** con controllo costante degli scostamenti budget
- **Analisi geografica per zona turistica e nazionalità clienti**
- **Ottimizzazione GOP e GOPPAR** tramite simulazioni di scenario
- Strumento di supporto per **decisioni manageriali data-driven**

---

## 🧾 Note e licenza
Il dataset è simulato a fini didattici e dimostrativi.  
Il file Power BI e i dati associati sono distribuiti con licenza **MIT**.

---

## 👤 Autore
**Riccardo Avitabile**  
Data Analyst | Business Intelligence | Power BI  
📧 *riccardoavitabile@example.com*  
📍 Italia  

