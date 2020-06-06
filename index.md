---
layout: default
title: Kurdish XeLaTeX Users Group
nav_order: 1
description: "Kurdish XeLaTeX Users Group homepage."
permalink: /
---

## Hûn bi xêr hatin
# Koma Bikarînerên XeLaTeX ya Kurdî
{: .fs-9 }

Armanca sereke ya vê komê, bi kar anîna sîstema nivîsa XeLaTeX ji bo nivîsandina zimanê Kurdî ye û jî afirandina platformek ji bo hêsan kirina hevkarî di nav civakên zanistî yên kurdan de ye.
{: .fs-6 .fw-300 }

<!-- [Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/pmarsceill/just-the-docs){: .btn .fs-5 .mb-4 .mb-md-0 } -->

---

## TeX çî ye?

[TeX](https://en.wikipedia.org/wiki/TeX){:target="_blank"} sîstema amade kirina nivîsê (*typesetting* bi Înglîsî) ye ku "ji bo afirandina pirtûkên xweşik û bi taybetî ji bo pirtûkên ku gelek matematîkê tê de heye" ye. Berevajî sîstemên din ên prose kirina nivîsan, mîna [Microsoft Word](https://en.wikipedia.org/wiki/Microsoft_Word){:target="_blank"} ku "*[what you see is what you get (WYSIWYG)](https://en.wikipedia.org/wiki/WYSIWYG){:target="_blank"}*" (bi Kurdî, "ya ku hûn dibînin, tiştê ku hûn digirin e") bikar tînin, nivîsandina li ser TeX bi bi karanîna nivîsa sade li gorî sintaksiya TeX pêk tê.

TeX di sala 1978-an de ji hêla zanyarê kompyutir, [Donald Knuth](https://en.wikipedia.org/wiki/Donald_Knuth){:target="_blank"} ve hat çêkirin. Armanca sereke ya TeX alîkariya karûbarê nivîsandinê ye. Nivîskaran divê xwedan amûran be ji bo nivîsandinê hemî tiştê ku dixwazin, helbest be, hevsengîyek kîmyewî be an formulek matematîkî. Gotina TeX ji peyva Yewnanî [τέχνη](https://en.wiktionary.org/wiki/%CF%84%CE%AD%CF%87%CE%BD%CE%B7){:target="_blank"} ye ku tê wateya *huner*ê. Ji ber ku fonema χ di kurdî de (û gelek zimanên din) tune ye, em dikarin bibêjin *têk* an *têx*, lê ne *têks*!

Hin taybetmendiyên sereke yên TeX wekê jêrîn in:

- Amadekirina kovar, pirtûk, raport, gotar û silaydên pêşkêşî
- Belgeyên mezin bi gelek beş û dabaşan rexistin
- Nivîsandina matematîkê û zanistên din û mijarên teknîkî
- Saz kirina bîbilyogirafî û referans dan bi hêsanî
- Bi kar anîna hêja ya materyalê girafîkî
- Veguheztina formatên din ên mîna HTML

Di bingeha TeX ê de, gelek sîstemek din hatine afirandin ji bo piştgiriya ziman û nivîsarên din. [LaTeX](https://en.wikipedia.org/wiki/LaTeX){:target="_blank"} û [XeLaTeX](https://en.wikipedia.org/wiki/XeTeX){:target="_blank"} du sîstemên bernas in ku îro bi berfirehî têne bikar anîn.

## XeLaTeX ji bo Kurdî

Berê, TeX tenê çend zimanan  bi tîpên Latînî piştgirî dikir û piştra, gelek ziman û nivîsar hatin zêde kirin. XeLaTeX li ser TeX hate afirandin û li [Unicode](https://en.wikipedia.org/wiki/Unicode){:target="_blank"} piştgirî dike. Kurdî gelek zarav û nivîsên wî hene û XeLaTeX ji bo wî sîstemek îdeal e, bi taybetî bi bikaranîna [`Polyglossia`](https://github.com/reutenauer/polyglossia){:target="_blank"}. Ji bo afirandina belgeyek bi XeLaTeX bi Kurdî, divê belgeya we wiha be:


```tex
\begin{lstlisting}
 \documentclass{article}
 \usepackage{polyglossia}

 \setdefaultlanguage[variant=kurmanji,script=latin,numerals=western]{kurdish}

 \begin{document}
 \end{documentu}
\end{lstlisting}
```

Di rêza yekem de, hûn dibêjin ku belgeya we gotarek e (`article`). Rêzên 2 heta 4 ji bo bi kar anîna `Polyglossia` ye û dibêjin ku dixwazin Kurmancî bi rênivîsa Latînî bi kar bînin. Kevala jêrîn sercem vebijarkên `Polyglossia` ji bo Kurdî nîşan dide.

| Polyglossia name        | variant          | script | numerals | 
|:-------------|:------------------|:------| :------- |
| Kurdish          | sorani | arabic, latin  | eastern, western |
| Kurdish | kurmanji  | arabic, latin  | eastern, western |

Bo nimûne, ger hûn dixwazin bi Soranî bi hejmarek tîpên Erebî û rênivîsa Erebî belgeyek çêbikin, hûn mîhengên xwe li rêza 4 wiha diguhezin:

```tex
 \setdefaultlanguage[variant=sorani,script=arabic,numerals=eastern]{kurdish}
 ```

Li versîyona niha ji `Polyglossia` **Soranî** û **Kurmancî** di her du tîpan **Erebî** and **Latînî** hene. Di derbarê salnameyê de, salnameya zayînî bi tenê heye. Bala xwe bidin ku du rewşan hene ji bo nîşan dana tarîxê: `\today` û `ontoday`. Li rewşê yekem de, tenê navê meha û hejmarên roj û sal tê, bo nimûne, *30 Gulan 2020*. Lê li rewşê paşîn, *ê* ya Îzafe jî tê, bo nimûne *30ê Gulanê 2020*. Vê vebijarkê tenê dema karanîna tîpên Latînî peyda dibe.

Ji bo zanyarîya zêdetir li ser `Polyglossia` û zimanê Kurdî, biçin [vir](https://kurdishxelatex.github.io/assets/Kurdish_XeLaTeX_English.pdf){:target="_blank"}.

## Belgeyan

Hûn dikarin belgeyên sade li ser cûreyên XeLaTeX bi zaravayên û nivîsarên cuda li jêr bibînin:

- Soranî bi rênivîsa Erebî: [XeLaTeX بۆ نووسینی کوردی]({{site.url}}/assets/Kurdish_XeLaTeX_Sorani_Arabic.pdf){:target="_blank"}
- Soranî bi rênivîsa Latînî: [XeLaTeX bo Nûsînî Kurdî]({{site.url}}/assets/Kurdish_XeLaTeX_Sorani_Latin.pdf){:target="_blank"}
- Kurmancî bi rênivîsa Latînî: [XeLaTeX ji bo nivîsandina Kurdî]({{site.url}}/assets/Kurdish_XeLaTeX_Kurmanji_Latin.pdf){:target="_blank"}
- Kurmancî bi rênivîsa Erebî: [XeLaTeX ژ بۆ نڤیساندنا کوردی]({{site.url}}/assets/Kurdish_XeLaTeX_Kurmanji_Arabic.pdf){:target="_blank"}

---

## Di derbarê projeyê de

Armanca me ya sereke di vê projeyê de çêkirina naverok bi Kurdî ji bo civakên zanistî yên kurdî ye. Hûn dikarin biçin malperên me bi [Soranî](https://kurdishxelatex.github.io/Sorani) and [Kurmancî](https://kurdishxelatex.github.io/Kurmanji). Dikarin **mijar û pirs**ên xwe li [https://github.com/KurdishXeLaTeX/Kurmanji/issues](https://github.com/KurdishXeLaTeX/Kurmanji/issues){:target="_blank"} binivîsin.

### Beşdarî

 Hûn dikarin ji hêla afirandina naverokê jî beşdarî vê komê bibin. 

<!-- Read more about becoming a contributor in [our GitHub repo](https://github.com/pmarsceill/just-the-docs#contributing). -->

<!-- #### Thank you to the contributors of the Kurdish XeLaTeX Users Group! -->

<!-- <ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul> -->

