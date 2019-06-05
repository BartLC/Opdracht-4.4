Ga na of er lege mappen in de backup staan en verwijder die dan. Dit is een uitbreiding op opdracht 4.3.



Get-ChildItem 'C:\data' -Recurse | Where-Object {$_.PSIsContainer -eq $true} | Where-Object {$_.GetFiles().Count -eq 0} | Remove-Item
