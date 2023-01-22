Dane o gruźlicy w różnych grupach pacjentów.
Lokalizacja oryginalnego pliku danych  :  folder OriginalData.
Lokalizacja przetworzonego pliku danych  :  folder AnalysisData i folder Documents.
Lokalizacja kodu potrzebnego do przetworzenia danych  :  folder CommandFiles, plik writtenCode.ipynb..
Lokalizacja przykładowej wizulacji danych dla wybranego kraju :  folder Documents, plik DataAppendix.ipynb.


Etapy przetwarzania danych:
1. Elimacja wierszy , gdzie kolumnach 'iso2' i 'year' znajdowały się Nan-wartości
2. ELimacja pustych wierszy.
3. Zamiana pozostałych NaN-wartości na 0.
4. Melting

Znaczenie symboli w przetworzonym pliku danych:
   'iso2' - identyfikator kraju  
   'year' - rok wystąpienia zakażenia
    'age' - wiek osoby chorej
   'f' - kobieta
   'm' - mężczyzna 
   'u' - nieznany
   '014'- wiek badanego w przedziale 0-14
   '1524'- wiek badanego w przedziale15-24
   '2534'- wiek badanego w przedziale 25-34
   '3544'- wiek badanego w przedziale 35-44
   '4554'- wiek badanego w przedziale 45-54
   '5564'- wiek badanego w przedziale 55-64
   '65'- wiek badanego 65+

Dane przetwarzano w języku Python w środowisku Visual Studio Code z użyciem biblioteki pandas.