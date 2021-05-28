## Standard-Befehl für neuen Registry-Eintrag erstellen:

`New-ItemProperty -Path "HKCU:\dummy\NetwrixKey" -Name "NetwrixParam" -Value ”NetwrixValue”  -PropertyType "String"`

## Existenz eines Schlüssels prüfen:
`Test-Path HKLM:\Software\Microsoft\"NET Framework Setup"\NDP`

## Neuen Schlüssel anlegen:
`New-Item HKCU:\Software\Microsoft\Test` -> der Schlüssel Test wird unter HKCU:\Software\Microsoft angelegt

## Neuen Wert anlegen:

`New-ItemProperty -Type DWord -Path HKCU:\Software\Microsoft\Test -Name Temp -value "1"` 

### Mögliche Typen des Wertes:
- DWord (REG_DWORD) 
- ExpandString (REG_EXPAND_SZ)
- Binary (REG_BINARY)
- String 
- MultiString (REG_MULTI_SZ)
- QWord (REG_QWORD)

## Einen Schlüssel löschen:
Remove-Item HKCU:\Software\Test -> der Schlüssel Test wird gelöscht

## Befehl für das Entfernen der Bing-Suche:

`New-ItemProperty -Path "HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer" -Name "DisableSearchBoxSuggestions" -Value ”1”  -PropertyType "DWORD"`

