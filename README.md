# Questionario Sicurezza PA - Delivery Care

Check-up gratuito conformità D.Lgs 81/08 per **Pubbliche Amministrazioni**.

## 🏛️ Caratteristiche

- **Target:** Comuni, Province, Regioni, Scuole, Università, ASL, Ministeri
- **15 domande** organizzate in 6 aree tematiche
- **Report istantaneo** con punteggio e criticità
- **Invio email** al richiedente + copia a Delivery Care
- **Tracking:** Google Analytics, Google Ads, Meta Pixel, Clarity

## 📁 Struttura

```
questionario-pa/
├── index.html      # Applicazione completa (single file)
└── README.md       # Documentazione
```

## 🚀 Deploy

Questo progetto è pensato per GitHub Pages:

1. Creare repository `questionario-pa` su GitHub
2. Caricare i file
3. Abilitare GitHub Pages (Settings → Pages → Branch: main)
4. Configurare DNS: `pa.deliverycare.it` → GitHub Pages

## ⚙️ Configurazione

### Formspree (invio email)

1. Registrarsi su [formspree.io](https://formspree.io)
2. Creare nuovo form con destinazione `info@deliverycare.it`
3. Copiare l'ID del form (es. `xabcdefg`)
4. Sostituire in `index.html`:
   ```javascript
   var FORMSPREE_URL="https://formspree.io/f/PLACEHOLDER_FORM_ID";
   ```
   con:
   ```javascript
   var FORMSPREE_URL="https://formspree.io/f/xabcdefg";
   ```

### DNS (pa.deliverycare.it)

Aggiungere record CNAME:
```
pa.deliverycare.it → deliverycaremeet-ctrl.github.io
```

## 📊 Aree Valutate

| Area | Punti Max | Contenuto |
|------|-----------|-----------|
| Sorveglianza Sanitaria | 20 | Medico competente, visite |
| Formazione | 30 | Generale, specifica, aggiornamento |
| Documenti | 10 | DVR |
| Nomine | 20 | RSPP, addetti emergenze |
| DPI e Sicurezza | 30 | DPI, piano emergenza, cassetta PS |
| Antincendio | 30 | Estintori, evacuazione, impianto elettrico |

**Punteggio totale:** 140 punti → normalizzato a 100

## 🎨 Personalizzazioni PA

Rispetto alla versione standard:
- Colore primario blu istituzionale (#1e40af)
- Badge "PA" nel header
- Settori specifici (Comuni, Scuole, ASL, etc.)
- Terminologia adattata (Ente, dipendenti pubblici, etc.)
- Sanzioni con riferimento a responsabilità dirigenziale
- CTA con riferimento a MEPA e Consip

## 📧 Contatti

**Delivery Care Srl - Società Benefit**  
P.zza centro commerciale 44, 20090 Segrate (MI)  
P.IVA 11263630961

📞 02 50047124  
📧 info@deliverycare.it

---

*Versione PA del questionario sicurezza - Marzo 2026*
