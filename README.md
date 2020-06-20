# Narzędzie do tworzenia poradników do gry Gwint
<h3>Opis pracy</h3><br>
Aplikacja webowa, której celem jest rozwijanie umiejętności i pomoc w lepszym zrozumieniu gry u graczy. W systemie są poszczególne grupy użytkowników:<br> <ul>
  <li>Moderator</li>
  <li>Gracz</li></ul>


  Moderator to doświadczony gracz, który ma dzielić się swoją wiedzą z innymi graczami. Może on dodawać nowe poradniki (ustalenie typu poradniku, dodanie kart do ręki gracza i na stół, opisanie efektu zagrania każdej karty z ręki). Moderator jest zalogowanym użytkownikiem.
  <br>Gracz po wejściu na stronę może wybrać kategorię z której chce się podszkolić. System losuje mu zadanie z danej kategotii. Zadanie to statyczny stan gry (stan stołu po obu stronach i ręka gracza). Po wybraniu karty, którą gracz chce zagrać system mówi mu czy decyzja była poprawna i daje dogłebne, analityczne podsumowanie sytuacji. 
  
<h3>Schemat bazy danych</h3>
<img src="https://github.com/Valithor/PracaDyplomowa/blob/master/BD.png">
<h3>Diagram przypadków użycia (z uwzględnieniem różnych aktorów)</h3>
<img src="https://github.com/Valithor/PracaDyplomowa/blob/master/DPU.png">
<h3>Opisy poszczególnych funkcjonalności (w postaci scenariuszy)</h3><br>
  
| Przypadek użycia  | Dodaj zadanie |
| ------------- | ------------- |
| Aktor  | Admin  |
| Scenariusz  | 1. Zalogowany admin przechodzi do eranu dodaj zadanie.<br> 2. System wyświetla ekran dodawania zadania. <br> 3. Admin uzupełnia dane (numer patcha, kategorię zadania, rękę gracza wraz z odpowiedziami na kliknięcie każdej karty) i stan stołu po stronie gracza i przeciwnika. <br> 4. System dodaje zadanie do bazy danych.|
| Wymagania  | Zalogowany użytkownik z uprawnieniami administratora.  |<br>
<!-- TABLE_GENERATE_END -->

  <!-- TABLE_GENERATE_START -->
| Przypadek użycia  | Wybierz kategorię |
| ------------- | ------------- |
| Aktor  | Użytkownik, System  |
| Scenariusz  | 1. Użytkownik wybiera kategorię, z której interesuje go zadanie.<br> 2. System losuje i wyświetla zadanie z określonej puli.|<br>
<!-- TABLE_GENERATE_END -->

  <!-- TABLE_GENERATE_START -->
| Przypadek użycia  | Rozwiąż zadanie |
| ------------- | ------------- |
| Aktor  | Użytkownik, System  |
| Scenariusz  | 1. Użytkownik wybiera odpowiedź. <br> 2. System wyświetla mu odpowiedź na jego wybór (odpowiedź zła/dobra, wyjaśnienie). <br> 3. Użytkownik powraca do ekranu głównego.|
| Alternatywne przebiegi zdarzeń  | 2a. Jeśli użytkownik jest zalogowany i odpowiedział poprawnie na pytanie system to zapisuje, aby nie pokazać tego samego zadania ponownie.  |
<!-- TABLE_GENERATE_END -->
<h3>Technologie</h3>
<ul>
  <li>React</li>
  <li>SpringBoot</li>
  <li>MySQL</li>
</ul>

<h3>Dokument zgłoszenia tematu</h3>
