# Mało Kreatywni - Projekt zespołowy ITM
Członkowie:
- Marcin Skorupski 161077
- Kamil Starczewski 169507
- Tomasz Szafrański 169510
- Szymon Sender 169492
- Bartłomiej Ślesiński 169512

Plik [Helpdesk_RAG.json](https://github.com/MarcinSkorupski/Malo-Kreatywni-ITM/blob/main/Helpdesk_RAG.json) zawiera flow, który można zaimportować w LangFLow. Aby działał poprawnie trzeba uruchomić lokalnie LangFlow i Ollamę oraz podać token bazy danych w Astra DB i wybrać odpowiednią kolekcję z danymi.
Aby Astra DB zawierała potrzebne dane należy po zalogowaniu stworzyć bazę danych "Serverless (Vector)" i stworzyć w niej kolekcję, najlepiej z domyślnym embeddingiem Nvidii służącym do obliczania wartości wektorowych i wyszukiwania. Następnie wybrać opcję "Load data" i "Structured data" i wrzucić plik [Szablon_HD_AI v2.csv](https://github.com/MarcinSkorupski/Malo-Kreatywni-ITM/blob/main/Szablon_HD_AI%20v2.csv) zawierający dane z pliku od ITM "Szablon_HD_AI (1).xlsx". Przed zakończeniem ładowania danych należy wybrać kolumnę do zwektorowania, w której będzie szukana podana fraza, czyli w tym przypadku najlepiej pasuje kolumna "Opis Błędu".
