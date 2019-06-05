---
# Translation instructions are after the "#" character in this first section. They are comments that do not show up in the web page. You do not need to translate the instructions after #.
# IN-PROGRESS

title: Éléments essentiels de l'accessibilité du Web # Do not translate "title:". Do translate the text after "title:".
nav_title: "Éléments de l'accessibilité du Web" # A short title that is used in the navigation
 
lang: fr   # Change "en" to the translated language shortcode from https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry
 
last_updated: 2019-06-05   # Put the date of this translation YYYY-MM-DD (with month in the middle)
translators:
- name: "@code-elegant"   # Replace @@ with translator name
# - name: "@@"   # Replace @@ with name, or delete this line if not multiple translators
# contributors:
# - name: "@@"   # Replace @@ with contributor name, or delete this line if none
# - name: "@@"   # Replace @@ with name, or delete this line if not multiple contributors
 
ref: /fundamentals/components/   # Do not change this
layout: default
github:
  repository: w3c/wai-components
  path: index.fr.md   # Add the language shortcode to the middle of the filename, for example index.fr.md
permalink: /fundamentals/components/fr   # Add the language shortcode to the end; for example /fundamentals/components/fr
feedbackmail: wai@w3.org

footer: >   # Translate all the words below, including "Date:" and "Editor:". Do not change these dates.
  <p>
    <strong>Autorisation d’exploitation&nbsp;:</strong>
    Vous pouvez utiliser les images de cette page pour l’éducation à l’accessibilité et son rayonnement si vous:<br>
    1. Incluez l’URI <strong><span class="changed">w3.org/WAI/fundamentals/components/</span> <em>en évidence</em></strong> à proximité de l’image, et <br>
    2. Incluez l’attribution à l’artiste, l’éditeur, et la mention de copyright dans tous les travaux publiés ou diffusés&nbsp;:<br><cite>Image par Michael Duffy, depuis: Essential Components of Web  Accessibility. Éditeur S.L. Henry. Copyright W3C <sup>®</sup> (MIT, ERCIM, Keio, Beihang). w3.org/WAI/fundamentals/components/</cite><br>
    Pour plus d’informations, voir <a href="https://www.w3.org/WAI/about/usingWAImaterial.html">Using WAI Materials (en anglais)</a>.
  </p>
  <p><strong>Date&nbsp;: </strong>Mis à jour le 27 February 2018. <!-- [<a href="@@">Changelog</a>] --> </p>
  <p><strong>Éditeur&nbsp;:</strong> <a href="http://www.w3.org/People/Shawn">Shawn Lawton Henry</a>. Graphiste&nbsp;: Michael Duffy.</p>
  <p>Élaboré avec des contributions du groupe de travail «&nbsp;Éducation et Rayonnement&nbsp;» (<span lang=”en”>Education and Outreach Working Group</span>) (<a href="http://www.w3.org/WAI/EO/">EOWG</a>).</p>
 
 
# Read Important Translations Guidance at https://www.w3.org/WAI/about/translating/#important
# Read Translations Notes for this resource at https://github.com/w3c/wai-components/blob/master/README.md
# end of translation instructions 
---

{::nomarkdown}
{% include box.html type="start" h="2" title="Résumé" class="full" %}
{:/}
 
Cette page montre comment l’accessibilité dépend de l’articulation harmonieuse de nombreux éléments, et comment des améliorations d’éléments particuliers pourrait améliorer sensiblement l’accessibilité du web.
 
Il fournit les bases pour comprendre les différents standards d’accessibilité produits par l’Initiative pour l’Accessibilité du Web (Web Accessibility Initiative WAI) du <abbr title="World Wide Web Consortium">W3C</abbr>.
 
{::nomarkdown}
{% include box.html type="end" %}
{:/}
 
{::nomarkdown}
{% include_cached toc.html type="start" title="Page Contents" class="simple" %}
{:/}
 
{::options toc_levels="2" /}
 
-   This text will be replaced by the TOC.
{:toc}
 
{::nomarkdown}
{% include_cached toc.html type="end" %}
{:/}
 
 
## Introduction {#intro}
{:.no_toc}
 
Il est essentiel que des éléments distincts et multiples du développement web et de l’interaction s’articulent convenablement pour que le Web soit accessible aux personnes handicapées. Ces éléments incluent&nbsp;:
 
-   **du contenu** - l’information contenue dans une page web ou une application web, y compris&nbsp;:
	-   de l’information primaire telle que du texte, des images et des sons,
	-   du code ou du balisage qui définit la structure, la présentation etc.&nbsp;;
-   **des navigateurs web, des lecteurs de média**, et d’autres «&nbsp;agents utilisateurs&nbsp;»&nbsp;;
-   **une technologie d’assistance**, dans certains cas – lecteurs d’écran, claviers alternatifs, contacteurs, logiciel de numérisation etc.&nbsp;;
-   les connaissances, l’expérience et dans certains cas les stratégies d’adaptation **des utilisateurs** pour l’utilisation du Web&nbsp;;
-   **des développeurs** - concepteurs, graphistes, codeurs, auteurs… y compris des développeurs handicapés et des utilisateurs qui contribuent&nbsp;;
-   **des outils de création** - logiciels de création de sites web&nbsp;;
-   **des outils d’évaluation** - outils d’évaluation de l’accessibilité web, validateurs HTML ou CSS…
 
## Comment les éléments s’articulent {#relate}
 
{% assign example_url = "/fundamentals/components/examples/#relate" | relative_url %}
![illustration montrant comment les éléments s’articulent, description détaillée à {{ example_url }}]({{ "/content-images/wai-components/relate.fr.png" | relative_url }}){:longdesc="{{example_url}}"}
 
Les **développeurs** web utilisent généralement **des outils de création** et des outils d’évaluation pour créer du **contenu** web.
 
**Les personnes** ("**utilisateurs**") utilisent des **navigateurs web, lecteurs de média, des technologies d’assistance,** ou d’autres "**agents utilisateurs**" pour obtenir ou interagir avec le **contenu**.
 
## Interdépendances entre les éléments {#depend}
 
Il y a des interdépendances importantes entre les éléments&nbsp;; c’est-à-dire que les éléments doivent s’articuler correctement pour que le web soit accessible. Par exemple, pour les équivalents textuels aux images&nbsp;:
 
-   les **spécifications techniques** traitent des équivalents textuels (par exemple, HTML définit l’attribut d’équivalent textuel (`alt`) pour l’élément image (`img`))
-   **les règles WAI** ([WCAG, ATAG, UAAG décrites ci-dessous](#guidelines)) - définissent comment mettre en place les équivalents textuels dans la perspective de l’accessibilité dans les différents éléments
-   les **développeurs** fournissent la formulation appropriée de l’équivalent textuel
-   les **outils de création** permettent, facilitent et promeuvent la fourniture d’un équivalent textuel dans une page web
-   les **outils d’évaluation** sont utilisés pour faciliter la vérification de la présence d’équivalents textuels
-   les **agents utilisateurs** fournissent des interfaces à destination des êtres humains et des machines pour l’équivalent textuel
-   les **technologies d’assistance** fournissent un accès aux êtres humains à l’équivalent textuel dans différentes modalités
-   les **utilisateurs** savent comment obtenir l’équivalent textuel depuis leur agent utilisateur ou leur technologie d’assistance ou les deux, selon que de besoin.
 
### Le cycle de mise en œuvre
 
Quand les fonctionnalités d’accessibilité sont réellement mises en œuvre dans un élément, les autres éléments sont plus susceptibles de les mettre en œuvre.
 
{% assign example_url = "/fundamentals/components/examples/#cycle" | relative_url %}
![illustration du cycle de mise en œuvre, description détaillée à {{ example_url }}]({{ "/content-images/wai-components/cycle.fr.png" | relative_url }}){:longdesc="{{example_url}}"}
 
- Quand **les navigateurs web, les lecteurs de média, les technologies d’assistance, et les autres agents utilisateurs** fournissent une fonctionnalité d’accessibilité, les utilisateurs sont plus susceptibles de l’exiger  et les développeurs sont plus susceptibles de l’implémenter dans leur **contenu**.
- Quand les développeurs veulent implémenter une fonctionnalité d’accessibilité dans leur **contenu**, ils sont plus susceptibles d’exiger que leur **outil de création** en rende simple la mise en œuvre.
- Quand **les outils de création** rendent simple la mise en œuvre d’une fonctionnalité, les développeurs sont plus susceptibles de la mettre en œuvre dans leur **contenu**.
- Quand une fonctionnalité d’accessibilité est mise en œuvre dans  **la plupart des contenus**, les développeurs et les utilisateurs sont plus susceptibles d’exiger que les **agents utilisateurs** la fournissent.
 
### Quand un élément est insuffisant
 
Si une fonctionnalité d’accessibilité n’est pas mise en œuvre dans un élément, il y a peu de motivation pour les autres éléments pour l’implémenter s’il n’en résulte pas une expérience utilisateur accessible. Par exemple les développeurs n’implémenteront pas une fonctionnalité d’accessibilité que les outils de création ne fournissent pas et que la plupart des navigateurs et des technologies d’assistance ne mettent pas en œuvre systématiquement.
 
{% assign example_url = "/fundamentals/components/examples/#weak" | relative_url %}
![illustration ce qui arrive quand un élément est insuffisant, description détaillée à {{ example_url }}]({{ "/content-images/wai-components/bridge.fr.png" | relative_url }}){:longdesc="{{example_url}}"}
 
Si un composant a une mise en œuvre de l’accessibilité amoindrie, d’autres éléments peuvent parfois compenser cela au travers de «&nbsp;contournements&nbsp;» qui nécessitent beaucoup plus d’effort et ne sont pas positifs pour l’accessibilité en général. Par exemple&nbsp;:
 
-   les développeurs ont plus de travail pour compenser des lacunes dans les fonctionnalités d’accessibilité dans les outils de création&nbsp;; par exemple en codant directement du balisage que grâce à un outil&nbsp;;
-   les utilisateurs peuvent avoir plus de travail pour compenser des lacunes dans les fonctionnalités d’accessibilité dans les navigateurs, les lecteurs de média, et la technologie d’assistance et le manque d’accessibilité du contenu&nbsp;; par exemple en utilisant différents navigateurs ou technologies d’assistance pour surmonter différents problèmes.
 
Cependant dans la plupart des cas les contournements ne sont pas mis en œuvre et le résultat reste décevant en termes d’accessibilité. De plus un support défaillant de l’accessibilité dans un élément ne peut parfois pas être raisonnablement compensé par les autres éléments et le résultat en est l’inaccessibilité, rendant impossible pour certaines personnes handicapées l’utilisation d’un site, une page ou une fonctionnalité précis.
 
## Règles et autres standards {#guidelines}
 
L’Initiative pour l’Accessibilité du Web (Web Accessibility Initiative ([WAI](https://www.w3.org/WAI/)) du World Wide Web Consortium ([W3C {% include_cached different.html %}](https://www.w3.org/)) développe des **standards d’accessibilité du web** pour différents éléments&nbsp;:
 
-   [[les règles pour l'accessibilité des outils d'édition / Authoring Tool Accessibility Guidelines (ATAG)]](/standards-guidelines/atag/) traite des outils de création ;
-   [[les règles pour l'accessibilité des contenus Web / Web Content Accessibility Guidelines (WCAG)]](/standards-guidelines/wcag/) traite du contenu web, et est utilisé par les développeurs, outils de création et outils d’évaluation de l’accessibilité ;
-   [[les règles pour l'accessibilité des agents utilisateurs / User Agent Accessibility Guidelines (UAAG)]](/standards-guidelines/uaag/) traite des navigateurs et lecteurs de média, y compris certains aspects des technologies d’assistance.
 
 
Ces règles d’accessibilité reposent sur le socle des spécifications techniques fondamentales du Web, et sont développées en coordination avec toutes les <a href="https://www.w3.org/TR/">spécifications techniques du W3C {% include_cached different.html %}</a> (HTML, CSS, SVG, SMIL, etc.). Le W3C développe aussi des spécifications techniques qui traitent directement d’accessibilité, y compris :
 
* la suite des spécifications [ARIA, Les applications Internet riches accessibles / The Accessible Rich Internet Applications](/standards-guidelines/aria/), qui définit une façon de de créer des applications web plus accessibles aux personnes handicapées. Elle facilite notamment le développement de contenu dynamique et de contrôles d’interface utilisateur avancés avec Ajax, HTML, JavaScript et les technologies associées.
 
{% assign example_url = "/fundamentals/components/examples/#guide" | relative_url %}
![illustration montrant les règles pour les différents éléments, description détaillée disponible à {{ example_url }}]({{ "/content-images/wai-components/specs.fr.png" | relative_url }}){:longdesc="{{example_url}}"}
 
Pour plus d’informations, voir [[W3C Accessibility Standards Overview]](/standards-guidelines/).
