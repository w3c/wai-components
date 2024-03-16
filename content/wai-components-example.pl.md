---
# Translation instructions are after the "#" character in this first section. They are comments that do not show up in the web page. You do not need to translate the instructions after "#".
# In this first section, do not translate the words before a colon. For example, do not translate "title:". Do translate the text after "title:"
---
title: Opisy ilustracji w artykule Podstawowe komponenty dostępności Internetu
nav_title: Illustration Descriptions

lang: pl   # Change "en" to the translated language shortcode
last_updated: 2024-03-07   # Put the date of this translation YYYY-MM-DD (with month in the middle)

# translators: # remove from the beginning of this line and the lines below: "# " (the hash sign and the space)
- name: "Stefan Wajda"   

# contributors:
# - name: "Jan Doe"   # Replace Jan Doe with contributor name, or delete this line if none
# - name: "Jan Doe"   # Replace Jan Doe with name, or delete this line if not multiple contributors


github:
    repository: w3c/wai-components
    content/wai-components-example.pl.md  # Add the language shortcode to the middle of the filename, for example: content/wai-components-example.fr.md

permalink: /fundamentals/components/examples/pl   # Add the language shortcode to the end, with no slash at the end. For example /path/to/file/fr
ref: /fundamentals/components/examples/    # Do not change this

feedbackmail: wai@w3.org

---

{::nomarkdown}
{% include_cached toc.html type="start" title="Treść strony" class="simple" %}
{:/}

{::options toc_levels="2" /}

-   This text will be replaced by the TOC.
{:toc}

{::nomarkdown}
{% include_cached toc.html type="end" %}
{:/}

Na tej stronie opisano ilustracje w dokumencie “[[Podstawowe komponenty dostępności Internetu]](/standards/components/)” oraz prezentacji [Podstawowe komponenty dostępności Internetu](http://www.w3.org/WAI/intro/components-slides).

## Opis ilustracji przedstawiającej powiązania między komponentami {#relate}

![Ilustracje powiązania między komponentami]({{ "/content-images/wai-components/relate-pl.svg" | relative_url }})

Ilustracja przedstawia trzy graficznie oznaczone pola obrazujące treść i ludzi. Pośrodku na górze znajduje się pole oznaczone jako „treść” na którym są baletnica, zdjęcie dziecka, znacznik img, tekst, formularz, widżet pogody i wykres kołowy. Idąc od dołu z lewej strony, linia łączy  „twórców” z „treścią” na górze, przechodząc przez „narzędzia autorskie” i „narzędzia oceniające”. Idąc od dołu z prawej stronie, linia łączy „użytkowników” z „treścią” na górze, przechodząc przez „przeglądarki, odtwarzacze mediów” i „technologie wspomagające”.

## Opis ilustracji przedstawiająej cykl implementacji {#cycle}

![Ilustruje cykl implementacji]({{ "/content-images/wai-components/cycle-pl.svg" | relative_url }})

Od elementu „treść” na górze biegnie strzałka w lewo przez element „narzedzia autorskie” do elementu „treść” na dole oraz strzałka w prawo od elementu „treść” na dole przez „technologie wspomagające” i „programy użytkowników” do „treści na górze”.

## Opis ilustracji Gdy jeden komponent jest słaby  {#weak}

![Pokazuje, co się dzieje, gdy jeden komponent jest słaby]({{ "/content-images/wai-components/bridge-pl.svg" | relative_url }})

Ilustracja przedstawia trzy graficznie oznaczone pola obrazujące treść i ludzi. Pośrodku na górze znajduje się pole oznaczone jako „treść” na którym są baletnica, zdjęcie dziecka, znacznik img, tekst, formularz, widżet pogody i wykres kołowy. Idąc od dołu z lewej strony, linia łączy  „twórców” z „treścią” na górze, przechodząc przez „narzędzia autorskie”. Idąc od dołu z prawej stronie, linia łączy „użytkowników” z „treścią” na górze, przechodząc przez wiele „przeglądarek, odtwarzaczy mediów” i „technologii wspomagających”.

## Opis ilustracji Wytyczne dla różnych komponentów {#guide}

![Ilustracja przedstawia różne wytyczne dla różnych komponentów]({{ "/content-images/wai-components/specs-pl.svg" | relative_url }})

Ilustracja przedstawia trzy graficznie oznaczone pola obrazujące treść i ludzi. Pośrodku na górze znajduje się pole oznaczone jako „treść” na którym są baletnica, zdjęcie dziecka, znacznik img, tekst, formularz, widżet pogody i wykres kołowy. Idąc od dołu z lewej strony, linia łączy  „twórców” z „treścią” na górze, przechodząc przez „narzędzia autorskie” i „narzędzia oceniające”. Idąc od dołu z prawej stronie, linia łączy „użytkowników” z „treścią” na górze, przechodząc przez „przeglądarki, odtwarzacze mediów” i „technologie wspomagające”.

Poniżej znajdują się „Wytyczne dla dostępności", które obejmują „ATAG” ze strzałką wskazującą na „narzędzia autorskie” i „narzędzia oceniające”, „WCAG” wskazujące na „treść” oraz „UAAG” wskazujące na „przeglądarki, odtwarzacze mediów” i „technologie wspomagające”. Na samym dole „Specyfikacje techniczne (HTML, ARIA, CSS, SVG, SMIL itp.)" tworzą podstawę ze strzałką wskazującą na wytyczne dla dostępności.

{% comment %}
@@  This is a redundant section. Repeated the relate.png image, but added a different description. (commented by zwiastunsw) @@
## Components and Guidelines Illustration Description {#rel-guide}

![Illustration showing How Components
Relate]({{ "/content-images/wai-components/relate.png" | relative_url }})

Illustration with labeled graphics of boxes, content, and people. at the top center is a pie chart, an image, a form, and text, labeled “content” - underneath is WCA". coming up from the bottom left, a line connects “developers” through “authoring tools” - underneath is ATAG - and “evaluation tools” - underneath is EARL - to “content” at the top. coming up from the bottom right, a line connects “users” to “browsers, media players” - underneath is UAAG - and “assistive technologies” to “content” at the top. In the middle, bottom is WAI-ARIA.

{% endcomment %}

{% comment %}

@@ commenting out - image was used in presentation that is not on new site - leaving here in case we want to resurrect it in the future. @@
-->
## Interdependencies Between Components, Example Illustration Description {#example-alt}

![Illustration showing examples of how components
relate.]({{ "/content-images/wai-components/relate-example.jpg" | relative_url }})

Illustration with labeled graphics of boxes, content, and people. at the top center "content" and underneath it is a logo and a box with: `<img src="WAI-logo-pl.svg" alt="Web Accessibility Initiative logo">`. coming up from the bottom left, a line connects “developers” through “authoring tools” and “evaluation tools” to “content” at the top. between the “developer” and “authoring tools” is a dialog box titled: Image Tag Accessibility Attributes, a field titled: Alternative Text filled in with: Web Accessibility Initiative logo. coming up from the bottom right, a line connects “users” to “browsers, media players” and “assistive technologies” to “content” at the top. just up from the “user” is a speech bubble saying: Web Accessibility Initiative logo and a yellow box with: Web Accessibility Initiative logo. at the bottom is: `1.1 Provide a text equivalent for every non-text element` 

{% endcomment %}
