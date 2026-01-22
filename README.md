Assicurati di avere Homebrew installato. In Terminale:

```bash
brew --version
```

Se non c’è, installalo con:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Avvia powershell:

```powershell
pwsh
```

Copia il codice nel terminale:

```powershell
Clear-Host
[console]::CursorVisible = $false

$art = @(
" (•‿•) "
"<(   )>"
" /   \"
)

$x = 0
$y = 0
$dx = 1
$dy = 1

$width  = [console]::WindowWidth
$height = [console]::WindowHeight

try {
    while ($true) {
        Clear-Host

        for ($i = 0; $i -lt $art.Count; $i++) {
            [console]::SetCursorPosition($x, $y + $i)
            Write-Host $art[$i]
        }

        $x += $dx
        $y += $dy

        if ($x -le 0 -or $x -ge ($width - 10)) { $dx = -$dx }
        if ($y -le 0 -or $y -ge ($height - 5)) { $dy = -$dy }

        Start-Sleep -Milliseconds 60
    }
}
finally {
    [console]::CursorVisibl
```
Installa node

```brew install node```

Copia il codice nel terminale 

```node -e "setInterval(()=>process.stdout.write(Math.random()>0.5?'\\':'//'),1)"```


