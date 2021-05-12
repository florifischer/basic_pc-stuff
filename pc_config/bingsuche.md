Standard-Befehl für neuen Registry-Eintrag erstellen:

`New-ItemProperty -Path "HKCU:\dummy\NetwrixKey" -Name "NetwrixParam" -Value ”NetwrixValue”  -PropertyType "String"`



Befehl für das Entfernen der Bing-Suche:

`New-ItemProperty -Path "HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer" -Name "DisableSearchBoxSuggestions" -Value ”1”  -PropertyType "DWORD"`

