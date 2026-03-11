# MacOs

## Creazione dello script
Crea un file chiamato "ascii.py" in una cartella.

Copia e incolla:
```bash
import random

try:
    while True:
        print("/" if random.random() < 0.5 else "\\", end="")
except KeyboardInterrupt:
    pass
```
Salva.

## Esecuzione
Tasto destro sulla cartella dove il file è salvato e seleziona l'ultima voce "Servizi", poi "Nuovo terminale nella cartella".

Scrivi:
```bash
python3 ascii.py
```
Premi invio.

## Interruzione
Premi Control + C

<br/>
--- 
<br/>

# Windows

## Creazione dello script
Crea un file chiamato "ascii.ps1" in una cartella.

Copia e incolla:
```bash
while ($true) {
    $carattere = if ((Get-Random -Maximum 2) -eq 0) { "/" } else { "\" }
    Write-Host $carattere -NoNewline
}
```
Salva.

## Esecuzione
Tasto destro sulla cartella dove il file è salvato e seleziona "Apri nel terminale".

Scrivi:
```bash
.\ascii.py
```
Premi invio.

## Interruzione
Premi Control + C
