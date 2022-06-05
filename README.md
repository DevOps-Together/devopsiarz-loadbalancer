## Ważne

https://github.com/DevOps-Together/devopsiarz-loadbalancer/issues - zapytania, problemy, plany, dzienniczek postępów itp

Zacząłeś/aś pracę na swoim branchu? Otwórz od razu DRAFT Pull Request, by inni mogli pytać, doradzać, komentować: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request

## Co robimy tutaj?

W tym projekcie mamy za zadanie utworzyć tzw. load balancer - "przekierowywacz" requestów. Spójrz na pozostałe projekty:

- https://github.com/DevOps-Together/devopsiarz-webserver
- https://github.com/DevOps-Together/devopsiarz-api-server

Wyobraź sobie, że mamy już napisany `webserver` i `api-server`. Jednak na świat wystawimy je pod jednym adresem. Pod tym jednym adresem będzie działał właśnie ten load balancer. Zadanie tego programu jest proste, załóżmy dla przykładu, że działa od pod adresem `domena.com`:

- niemal wszelkie requesty z przeglądarki WWW, metodą GET np. `domena.com` czy `www.domena.com` są kierowane do `webserver`. Webserver serwuje pliki, zwraca odpowiedź, a load balancer "przekazuje" tę odpowiedź klientowi
- wszelkie requesty z uri=`/wiadomosc` są jedynym wyjątkiem i one są przekazywane do `api-server` z kolei, który już wie, co z `/wiadomosc` ma zrobić

Pamiętaj: nie musisz czekać aż `webserver` czy `api-server` będą gotowe i działające. Możesz je "zasymulować" i w ten sposób testować load balancer właśnie.

### Minimalna funkcjonalność:

- przekazywanie właściwych requestów do/z webserwera (patrz opis wyżej)
- przekazywanie właściwych requestów do/z api-server (patrz opis wyżej)

### Sposób rozwiązywania
- tworzysz swój branch, na którym tworzysz rozwiązanie, kod na branchu nie musi działać dobrze, ani działać wcale - to jest nauka
- jak stworzysz branch - **otwórz od razu Pull Request**, aby na nim pracować i przyjmować uwagi
- jak nie wiesz, jak ruszyć - pytaj w Issues lub na kanale #projekt-devopsiarz na Discordzie
- język dowolny, jak chcesz się nauczyć, to zacznij w języku, w który chcesz wejść (kiedyś trzeba)

### Pomocne linki - tutaj rzucamy linki, które mogą pomóc nam lub innym
[Jak tworzyć Pull Request na GitHub - EN](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
