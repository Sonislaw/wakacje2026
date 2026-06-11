<!DOCTYPE html>
<html lang="pl">
<head>
<meta charset="UTF-8">
<title>Odliczanie dni do wakacji</title>
<style>
body { font-family: Arial, sans-serif; margin: 20px; line-height: 1.6; }
#countdown { font-size: 2em; margin: 20px 0; }
#phrase, #fact { font-size: 1.2em; margin: 15px 0; }
#progress-bar { margin: 20px 0; }
progress { width: 100%; height: 1em; }
.milestones { list-style: none; padding: 0; }
.milestones li { display: inline-block; margin-right: 1em; }
#photo { margin: 20px 0; }
#photo img { max-width: 100%; height: auto; }
</style>
</head>
<body>
<h1>Odliczanie dni do wyjazdu</h1>
<div id="countdown" aria-label="Pozostały czas"></div>
<div id="phrase" aria-live="polite"></div>
<div id="fact" aria-live="polite"></div>
<div id="progress-bar">
  <label for="progress">Procent odbytego czasu:</label>
  <progress id="progress" value="0" max="100"></progress>
</div>
<ul id="milestones" class="milestones" aria-label="Kamienie milowe"></ul>
<div id="photo">
  <h2>Zdjęcie dnia</h2>
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/48/Ocean_sunrise_%28Unsplash%29.jpg" alt="Zdjęcie plaży o zachodzie słońca" />
</div>
<script>
// Lista tekstów motywacyjnych
var phrases = [
  "Już tylko 62 dni do wyjazdu - ciesz się każdym z nich!",
  "Odliczanie: 61 dni do wakacyjnej przygody!",
  "Za 60 dni zajmiesz się relaksem i przyjemnościami.",
  "Zostało 59 dni - prawdziwa radość nadchodzi!",
  "Pozostało 58 dni do Twojego urlopu - baw się dobrze!",
  "Już 57 dni i będziesz wśród natury.",
  "Tylko 56 dni dzieli Cię od marzeń.",
  "Wkrótce się zaczyna: 55 dni!",
  "Świetna wiadomość: 54 dni do wakacji!",
  "Już niecierpliwie wyczekujesz 53 dni!",
  "Za 52 dni spakujesz walizki.",
  "Za 51 dni zacznie się Twoja przygoda.",
  "Witaj w odliczaniu: zostało 50 dni.",
  "Każdy dzień zbliża cię do celu: zostało 49 dni.",
  "49 dni - czujesz już letni klimat?",
  "48 dni i zapomnisz co to stres!",
  "Na horyzoncie wakacji zostało 47 dni.",
  "Już 46 dni, a wakacje nadchodzą wielkimi krokami!",
  "Za 45 dni… Twoja głowa pomalowana słońcem.",
  "Odliczanie trwa: 44 dni!",
  "Już 43 dni i odrzucisz kalendarz.",
  "Nadchodzi radosny czas: zostało 42 dni.",
  "Szansa oderwania się od rzeczywistości: 41 dni.",
  "Pozostało tylko 40 dni do wielkiego wypoczynku!",
  "Nie patrz w tył: zostało 39 dni do przodu!",
  "Przed Tobą 38 dni beztroski.",
  "Już 37 dni czystej przyjemności przed nami.",
  "Jedziemy za 36 dni!",
  "Nie martw się, zostało tylko 35 dni!",
  "Zostało 34 dni, a wakacje są tuż tuż!",
  "Przywitaj wakacje: zostało 33 dni.",
  "32 dni i udamy się w nieznane!",
  "Widok wakacji już blisko: 31 dni.",
  "Tylko 30 dni, potem – pełen luz!",
  "W radości odliczamy 29 dni.",
  "Ten moment nadchodzi: 28 dni.",
  "Na drogowskazach – 27 dni do wakacji.",
  "Za 26 dni spełnią się Twoje letnie marzenia.",
  "Za 25 dni czas w pracy zamienisz na drinka na plaży.",
  "Wypoczynek za 24 dni – cel jest blisko.",
  "23 dni: czas szybciej nie może płynąć!",
  "Za 22 dni budzik nie zadzwoni, tylko słońce wstanie.",
  "Do wakacji: 21 dni.",
  "20 dni – pozytywna niespodzianka czeka.",
  "19 dni do szczęścia!",
  "Za 18 dni zatracisz się w letnich przygodach.",
  "Od dziś Twoje ulubione pytanie: zostało 17 dni?",
  "16 dni – już prawie tam!",
  "Wkrótce koniec odliczania: zostało 15 dni.",
  "Za 14 dni wyjazd – pakuj się powoli!",
  "13 dni i rozpocznie się Twój urlop.",
  "Już 12 dni i świętujemy wakacje!",
  "11 dni i omijasz budzik szerokim łukiem.",
  "Za 10 dni zamienisz stres na plażową leżankę.",
  "9 dni od teraz: stań przed przygodą.",
  "Tylko 8 dni i długie dobre samopoczucie.",
  "Ciesz się odliczaniem: zostało 7 dni.",
  "5 dni - od rana do wieczora plażą!",
  "4 dni – dzień po dniu bliżej celu.",
  "Zostały jeszcze 3 dni!",
  "Zostały jeszcze 2 dni!",
  "Jutro zaczyna się Twoja przygoda!"
];
// Lista ciekawostek
var facts = [
  // Legoland (Germany)
  "LEGOLAND Deutschland Resort położony jest w Günzburgu (Bawaria), tuż przy autostradzie A8 między Stuttgartem a Monachium.",
  "Park otwarto 17 maja 2002 roku, jest jednym z największych parków rozrywki w Niemczech.",
  "Ma powierzchnię ok. 43 ha i oferuje 68 atrakcji w 11 tematycznych krainach z ponad 58 mln klocków LEGO®.",
  "Miniland w tym parku prezentuje największe niemieckie i europejskie budowle (Neuschwanstein, Zamek w Malborku, budynki Berlina) zbudowane z 25 mln klocków LEGO®.",
  "Od 2024 obok LEGOLANDU znajduje się pierwszy w Europie park tematyczny Peppa Pig Park (otwarty 19 maja 2024).",
  "W pobliżu znajduje się także wioska wakacyjna z hotelami i kempingiem: można nocować m.in. w hotelu Wyspa Piratów, tematycznych domkach wakacyjnych, zamkach rycerskich lub na polu kempingowym.",
  // Olandia (Poland)
  "Olandia leży w Prusimiu (woj. wielkopolskie) w Krainie 100 Jezior, nad jeziorem Olandia, w otulinie Puszczy Noteckiej.",
  "Ośrodek zajmuje 6 ha, ma kameralną atmosferę i oferuje 60 pokoi w stylu rustykalnym oraz 15 stanowisk dla kamperów nad samym brzegiem jeziora (z prądem i wodą).",
  "Na terenie ośrodka znajduje się prywatna plaża, SPA, kort tenisowy, boiska sportowe, stajnie, pole do minigolfa, skansen miniatur oraz zabytkowe wiatraki i mini-zoo.",
  "Działa tutaj restauracja „Olenderskie Smaki” z daniami kuchni regionalnej inspirowanymi tradycjami Holendrów osiedlających się niegdyś w Polsce.",
  "W sezonie letnim organizowane są animacje wodne, warsztaty kulinarne oraz kino familijne, a od lata 2022 planowane jest otwarcie krytego basenu.",
  // Camping Sobec (Slovenia)
  "Camping Šobec położony jest w Lescach, ok. 3 km od Jeziora Bled, u podnóża Alp Julijskich i Pasma Karawank.",
  "Ośrodek otacza woda – z trzech stron graniczy z rzeką Sava Dolinka, a z czwartej strony z małym sztucznym jeziorem z wyznaczoną strefą do kąpieli.",
  "Ma ok. 500 miejsc kempingowych (457 z przyłączem prądu) i oferuje plac zabaw, supermarket, bar/restaurację oraz bezpłatne Wi-Fi na całym terenie.",
  "Region obfituje w atrakcje outdoorowe – rzeki Sava Dolinka i Bohinjka nadają się do kajakarstwa i raftingu, a góry – do wspinaczki, paralotniarstwa i canyoningu.",
  "Camping Šobec zdobył liczne nagrody: w 2023 zajął 1. miejsce w rankingu Avtokampi oraz tytuł Najlepszego Kempingu w Słowenii.",
  "Ma także certyfikat ekologiczny Green Key za naturalne kąpielisko i działa od ponad 68 lat, goszcząc już ponad 2 mln zadowolonych gości.",
  // San Marino Camping Valamar (Croatia)
  "Camping San Marino położony jest w Loparze na wyspie Rab, przy piaszczystej Rajskiej Plaży (Paradise Beach) – plaży o długości ok. 1500 m, wyróżnionej Błękitną Flagą.",
  "Na terenie ośrodka są nowoczesne parcele, mobilne domki („Lopar Garden Homes”) i pokoje w hotelu, wszystko kilkadziesiąt metrów od brzegu morza.",
  "Działa tu główna restauracja i kilka bufetów serwujących kuchnię śródziemnomorską (pizza, makarony, grill, owoce morza) oraz beach bary, a także piekarnia i sklep spożywczy.",
  "Dla dzieci dostępny jest Maro Mini Club i dmuchany park wodny, a dla dorosłych – centrum SPA, boiska (m.in. do siatkówki plażowej) i zajęcia sportowo-rekreacyjne.",
  "Na samej plaży wypożyczysz kajaki lub rowerki wodne, pograsz w siatkówkę plażową albo wejdziesz do Aquaparku z dmuchanymi zjeżdżalniami."
];
// Obliczenia licznika
function updateCountdown() {
    var now = new Date();
    var target = new Date(Date.UTC(2026,7,12));
    target = new Date(target.getTime() + target.getTimezoneOffset()*60000);
    var diff = target - now;
    var days = Math.floor(diff/(1000*60*60*24));
    if (days < 0) days = 0;
    document.getElementById("countdown").textContent = days + " dni do wyjazdu!";
    // pasek postępu
    var start = new Date(); start.setFullYear(2026,5,11);
    var total = target - start;
    var elapsed = now - start;
    var percent = Math.min(100, Math.floor(elapsed/total * 100));
    document.getElementById("progress").value = percent;
    // kamienie milowe
    var steps = [100,90,75,50,30,14,7,1];
    var milestones = document.getElementById("milestones");
    milestones.innerHTML = "";
    steps.forEach(function(s){
        if (s <= days) {
            var li = document.createElement("li");
            li.textContent = s + " dni";
            milestones.appendChild(li);
        }
    });
}
// Losowanie frazy i ciekawostki
function randomize() {
    var idx = Math.floor(Math.random() * phrases.length);
    document.getElementById("phrase").textContent = phrases[idx];
    var j = Math.floor(Math.random() * facts.length);
    document.getElementById("fact").textContent = facts[j];
}
document.addEventListener("DOMContentLoaded", function(){
    updateCountdown();
    randomize();
});
</script>
</body>
</html>
