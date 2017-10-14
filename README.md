# raupjc-hw0
C# development course HW #0
# Pitanje 1:
Stvorila se .dll datoteka za library klasu.
Vraća se UnhandledException jer nedostaje klasni .dll.
To se događa jer prevedena aplikacija pokušava dohvatiti prevedeni kod iz .dll containera, ali ga ne može naći, zbog čega se izbacuje exception.
Poslati ću vam .exe datoteku glavnog programa i .dll (koji se u mojem slučaju zovu Test.exe i Class000.dll).
# Pitanje 2:
U slučaju kada se debuggao samo Test.exe, prikazivao je izmjenjeni string. To je zato jer je VS automatski izgradio izmijenjeni Class000 library, jer Test projekt ovisi o njemu. No, kada se bez prevođenja pokrenuo Test.exe, prikazivao se stari string, jer .dll nije ponovo izgrađen.
# Pitanje 3:
Build se izvršava normalno kao i obično, a NodaTime je nadodan u packages folder.