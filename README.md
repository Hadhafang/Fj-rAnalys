# Fj-rAnalys
Kod för att analysera filer från ESA sentinel
Ska svar på hur stor del av en tile som är molnig
Om en tile är hel

33WRX, 34VDR verkar trasig

iterateMapp.py är ett första försök till att iterera genom en mapp för att hitta rätt fil. I vår fall filer innehållandes metadata

iterateFolder.py extraherar information om molnighet i angiven mapp. Funktionen hittar alla filer som avslutas med ".xml" samt innehåller texten "MTD". För varje mapp hittas tre sådana filer (endast en behövs). För varje fil hittas elementet "Cloud_Coverage_Assessment" och dess värde returneras.
