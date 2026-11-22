# Sito azienda: come pubblicarlo su GitHub Pages

Contenuto della cartella:

- `index.html`: home
- `pacchetti.html`: pacchetti e prezzi
- `contatti.html`: pagina "Parliamo del tuo progetto" con il modulo
- `style.css`: stile e animazioni (condiviso da tutte le pagine)
- `.nojekyll`: file vuoto, dice a GitHub di pubblicare i file così come sono

## 1. Completa i segnaposto

Apri i file con un editor di testo (anche il Blocco note) e cerca le parole tra parentesi quadre:

- `[Nome azienda]` (in tutte le pagine, intestazione e piè di pagina)
- `[€ prezzo]` (pacchetti.html)
- `[email aziendale]`, `[@profilo Instagram]`, `[lun–ven, 9–18]`, `[città]` (contatti.html)
- `P.IVA [numero]` (piè di pagina di tutte le pagine)

Nel piè di pagina "Privacy policy" e "Cookie policy" sono solo testo: prima di pubblicare servono pagine vere e collegamenti a quelle pagine. Conviene farle preparare da un professionista.

## 2. Collega il modulo di contatto

GitHub Pages ospita solo pagine statiche, quindi il modulo ha bisogno di un servizio che riceva i messaggi e li giri alla tua email. Con Formspree (gratuito per pochi invii al mese):

1. Registrati su https://formspree.io e crea un nuovo modulo.
2. Copia l'indirizzo che ti danno, simile a `https://formspree.io/f/abcdwxyz`.
3. In `contatti.html` cerca `INSERISCI_ID` e sostituisci tutto l'indirizzo con il tuo.

Altri servizi simili funzionano allo stesso modo (per esempio Web3Forms o Getform).

## 3. Pubblica su GitHub

1. Crea un account su https://github.com.
2. Clicca **New repository**, scegli un nome (per esempio `sito-azienda`) e lascialo **Public**.
3. Nel repository clicca **Add file → Upload files**, trascina dentro tutti i file di questa cartella (compreso `.nojekyll`) e clicca **Commit changes**.
4. Vai in **Settings → Pages**. In "Branch" scegli `main` e la cartella `/ (root)`, poi **Save**.
5. Dopo uno o due minuti il sito è online su `https://TUONOME.github.io/NOME-REPOSITORY/`.

## 4. Dominio personalizzato (facoltativo)

In **Settings → Pages → Custom domain** inserisci il tuo dominio e segui le istruzioni per i record DNS sul sito dove lo hai comprato.

## Per cambiare il colore principale

In `style.css`, in cima, cambia il valore di `--ac` (ora `#2F3CF0`). Per esempio `#0B7A5C` per un verde.
