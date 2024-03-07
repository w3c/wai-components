---
# Translation instructions are after the "#" character in this first section. They are comments that do not show up in the web page. You do not need to translate the instructions after #.
# In this first section, do not translate the words before a colon. For example, do not translate "title:". Do translate the text after "title:"

title: Podstawowe komponenty dostępności Internetu
nav_title: "Komponenty dostępności Internetu" # A short title that is used in the navigation

lang: pl   # Change "en" to the translated language shortcode from https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry

last_updated: 2024-03-05   # Put the date of this translation YYYY-MM-DD (with month in the middle)

translators:
  - name: "Stefan Wajda"

github:
  repository: w3c/wai-components
  path: content/index.pl.md   # Add the language shortcode to the middle of the filename, for example index.fr.md

permalink: /fundamentals/components/pl 
ref: /fundamentals/components/   # Do not change this
 
feedbackmail: wai@w3.org

# In the footer below:
# Do not change the dates
# Translate the other words, including "Date:" and "Editor:"
# Translate the Working Group name. Leave the Working Group acronym in English.
footer: >
  <p>
    <strong>Zgoda na wykorzystanie:</strong> 
    Obrazów zamieszczonych na tej stronie można używać w celach edukacyjnych i informacyjnych, jeśli:<br> 
    1. Umieścisz URI <strong><span class="changed">w3.org/WAI/fundamentals/components/</span> <em>w widocznym miejscu</em></strong> w pobliżu obrazu, oraz <br>
    2. Umieścisz informacji o artyście, redaktorze i prawach autorskich we wszelkich publikowanych lub zamieszczanych materiałach:<br>
    <cite>Autor grafik Michael Duffy, źródło: Podstawowe komponenty doostępności Internetu. S.L. Henry, ed. Copyright W3C <sup>®</sup> (MIT, ERCIM, Keio, Beihang). w3.org/WAI/fundamentals/components/</cite><br>
    Aby uzyskać więcej informacji, zobacz <a href="https://www.w3.org/WAI/about/using-wai-material/">Using WAI Materials</a>.
  </p>
  <p><strong>Data: </strong>Updated 27 February 2018.</p>
  <p><strong>Redaktor:</strong> <a href="https://www.w3.org/People/Shawn">Shawn Lawton Henry</a>. Autor grafik: Michael Duffy.</p>
---

{::nomarkdown}
{% include box.html type="start" h="2" title="Podsumowanie" class="full" %}
{:/}

Ta strona pokazuje, w jaki sposób dostępność internetowa zależy od kilku współpracujących ze sobą komponentów oraz w&nbsp;jaki sposób ulepszenia w&nbsp;określonych komponentach mogą znacznie poprawić dostępność internetową.

Stanowi on podstawę do zrozumienia różnych standardów dostępności opracowanych przez Inicjatywę na Rzecz Dostępności Internetowej (WAI), która jest częścią Konsorcjum <abbr title="World Wide Web">W3C</abbr>.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::nomarkdown}
{% include_cached toc.html type="start" title="Treść strony" class="simple" %}
{:/}

{::options toc_levels="2" /}

-   This text will be replaced by the TOC.
{:toc}

{::nomarkdown}
{% include_cached toc.html type="end" %}
{:/}


## Wprowadzenie {#intro}
{:.no_toc}

Aby Internet był dostępny dla osób z niepełnosprawnościami, konieczne jest współdziałanie kilku różnych komponentów związanych z&nbsp;projektowaniem i&nbsp;tworzeniem treści cyfrowych. Te komponenty to:

-   **treść** - informacje na stronie internetowej lub w aplikacji internetowej, w tym:
    -   informacje naturalne (takie jak tekst, obraz i dźwięki) oraz
    -   kod lub znaczniki definiujące strukturę, prezentację itp.
-   **przeglądarki internetowe, odtwarzacze multimedialne**, i inne „programy użytkownika”
-   **technologie wspomagające**, w niektórych przypadkach - czytniki ekranu, alternatywne klawiatury, przełączniki, oprogramowanie skanujące itp.
-   **użytkownicy**, ich wiedza, doświadczenia, a w niektórych przypadkach, sposób korzystania z internetu (strategie adaptacyjne
-   **twórcy** - projektanci, programiści, autorzy itd., w tym projektanci z niepełnosprawnościami i&nbsp;użytkownicy, którzy współtworzą treść
-   **narzędzia autorskie** - oprogramowanie do tworzenia treści cyfrowych
-   **narzędzia oceniające** - oprogramowanie do oceny dostępności cyfrowej, walidatory HTML i CSS itp.

## Jak komponenty są ze sobą powiązane {#relate}

{% assign example_url = "/fundamentals/components/examples/#relate" | relative_url %}
![Ilustruje powiązanie komponentów, szczegółowy opis na stronie {{ example_url }}]({{ "/content-images/wai-components/relate.png" | relative_url }}){:longdesc="{{example_url}}"}

**Twórcy** stron internetowych zwykle używają **narzędzi autorskich** i narzędzi oceny do tworzenia **treści** cyfrowych.

**Ludzie** („**użytkownicy**”) używają **przeglądarek, odtwarzaczy medialnych, technologii wspomagających** lub innych „**programów użytkownika**”, aby uzyskać dostęp do treści cyfrowych i&nbsp;wchodzić z&nbsp;nimi w&nbsp;interakcje.

## Współzależności komponentów {#depend}

Między tymi komponentami istnieją istotne współzależności; to znaczy że komponenty muszą ze sobą współpracować, aby sieć internetowa była dostępna. Na przykład, dla alternatywnego tekstu opisującego obraz:

-   **specyfikacja techniczna** wymaga alternatywnego tekstu (np. HTML definiuje atrybut alternatywnego tekstu (`alt`) w elemencie obrazka (`img`)
-   **wytyczne WAI** - WCAG, ATAG i UAAG, wymienione w dalszej części - określają, jak zaimplementować tekst alternatywny, aby zwiększyć dostępność w różnych komponentach
-   **twórcy** zapewniają odpowiednie alternatywne sformułowania tekstu
-   **narzędzia autorskie** umożliwiają, ułatwiają i promują zamieszczanie alternatywnego tekstu na stronie internetowej
-   **narzędzia oceny** służą do sprawdzenia, czy istnieje tekst alternatywny
-   **oprogramowanie użytkownika** zapewnia ludziom i maszynom interfejs do tekstu alternatywnego w&nbsp;różnych trybach
-   **użytkownicy** wiedzą jak odczytać alternatywny tekst w&nbsp;wykorzystywanym przez nich oprogramowaniu i/lub technologiach wspomagających, w razie potrzeby
	  
### Cykl wdrożeniowy

Gdy funkcje dostępności zostaną skutecznie zaimplementowane w jednym komponencie, istnieje większe prawdopodobieństwo, że zostaną wdrożone w innych komponentach.

{% assign example_url = "/fundamentals/components/examples/#cycle" | relative_url %}
![Ilustruje cykl implementacji komponentów dostępności cyfrowej opisany poniżej, szczegółowy opis w {{ example_url }}]({{ "/content-images/wai-components/cycle.png" | relative_url }}){:longdesc="{{example_url}}"}

- Gdy **przeglądarki internetowe, odtwarzacze multimedialne, technologie wspomagające** i inne **programy użytkownika** obsługują funkcje dostępności, użytkownicy częściej będą tego wymagać, a programiści implementować je w swoich **treściach**.
- Gdy twórcy chcą wdrożyć funkcje dostępności w swoich **treściach**, częściej domagają się, aby **narzędzie autorskie** ułatwiało ich wdrożenie. 
- Gdy **narzędzia autorskie** umożliwiają łatwą implementację funkcji dostępności, twórcy chętniej je zaimplementują w swoich **treściach**. 
- Gdy funkcje dostępności są zaimplementowane na **większości treści**, twórcy i&nbsp;użytkownicy częściej żądają, aby **programy użytkownika** je obsługiwały.

### Gdy jeden komponent jest słaby

Jeśli funkcje dostępności nie są zaimplementowane w którymś z komponentów, motywacja do zaimplementowania ich w&nbsp;pozostałych komponentach spada, jeśli nie skutkuje to zwiększeniem dostępności dla użytkownika. Na przykład mało prawdopodobne jest, aby programiści wdrożyli funkcję dostępności, która nie jest obsługiwana przez narzędzia autorskie i której nie wspiera większość przeglądarek lub technologii wspomagających.

{% assign example_url = "/fundamentals/components/examples/#weak" | relative_url %}
![Ilustruje, co dzieje się, gdy jeden komponent jest słaby, szczegółowy opis w {{ example_url }}]({{ "/content-images/wai-components/bridge.png" | relative_url }}){:longdesc="{{example_url}}"}

Gdy jeden z komponentów w niewystarczającym stopniu wspiera dostępność, czasem inne komponenty mogą te niedostatki zrekompensować poprzez „obejścia”, choć wymaga to znacznie większego wysiłku i ogólnie nie jest dobre dla dostępności. Na przykład:

-   twórcy mogą wykonać więcej pracy, aby zrekompensować brak wsparcia dostępności w&nbsp;narzędziach autorskich; na przykład poprzez bezpośrednie kodowanie znaczników zamiast za pomocą narzędzia,
-   użytkownicy mogą wykonać więcej pracy, aby zrekompensować niedostateczne wsparcie dostępności w przeglądarkach, odtwarzaczach mediów lub technologiach wspomagających; na przykład, używając innej przeglądarki lub technologii wspomagającej w celu przezwyciężenia różnych problemów z dostępnością

Jednak w większości przypadków obejścia nie są możliwe, a efekt jest wciąż niezadowalający. Ponadto czasami słabe wsparcie dostępności w jednym komponencie nie może być sensownie rozwiązane przez inny komponent, czego rezultatem jest niedostępność, uniemożliwiająca niektórym osobom z niepełnosprawnościami korzystanie z określonej witryny, strony lub funkcji.

## Wytyczne i inne standardy {#guidelines}

Inicjatywa na Rzecz Dostępności Internetowej [WAI](https://www.w3.org/WAI/)) w Konsorcjum <span lang="en">World Wide Web</span> ([W3C](https://www.w3.org/)) opracowuje **standardy dostępności cyfrowej** dla różnych komponentów:

-   [[Wytyczne dla dostępności narzędzi autorskich (ATAG)]](/standards-guidelines/atag) dotyczące narzędzi do tworzenia treści
-   [[Wytyczne dla dostępności internetowej (WCAG)]](/standards-guidelines/wcag/) dotyczące treści i wykorzystywane przez twórców oraz narzędzia autorskie i oceniające
-   [Wytyczne dla dostępności programów użytkownika (UAAG)](/standards-guidelines/uaag/) dotyczące przeglądarek i odtwarzaczy multimedialnych oraz niektórych aspektów technologii wspomagających

Te wytyczne opierają się na podstawowych specyfikacjach technicznych Internetu i są opracowywane w połączeniu ze <a href="https://www.w3.org/TR/">wszystkimi specyfikacjami technicznymi W3C</a> (HTML, CSS, SVG, SMIL itp.). W3C opracowuje również specyfikacje techniczne, które bezpośrednio dotyczą dostępności, w tym:

* [ARIA, Złożone Dostępne Aplikacje Internetowe](/standards-guidelines/aria/), która wskazuje, jak uczynić złożóne aplikacje internetowe bardziej dostępnymi dla osób z&nbsp;niepełnosprawnościami. Szczególnie pomaga w tworzeniu treści dynamicznych i zaawansowanych kontrolek interfejsu użytkownika opracowanych przy użyciu Ajax, HTML, JavaScript i&nbsp;pokrewnych technologii.

{% assign example_url = "/fundamentals/components/examples/#guide" | relative_url %}
![Pokazuje wytyczne dla różnych komponentów, szczegółowo opisane w {{ example_url }}]({{ "/content-images/wai-components/specs.png" | relative_url }}){:longdesc="{{example_url}}"}

Aby uzyskać więcej informacji, zobacz [[Omówienie standardów dostępności W3C]](/standards-guidelines/).
