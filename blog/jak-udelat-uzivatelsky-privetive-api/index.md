---
title: Uživatelem jsou i AI agenti
author: Honza Soukup
url: https://www.honzasoukup.cz/blog/jak-udelat-uzivatelsky-privetive-api
language: cs
published: 2024
updated: 2026-10-04
---

# Uživatelem jsou i AI agenti

Autor: Honza Soukup, UX v době AI

V roce 2024 jsem psal, že programátoři jsou taky lidi a API potřebuje dobré UX. Dnes je ten uživatel ještě jiný: váš web a API čtou AI agenti. Hledají za lidi, porovnávají, objednávají. Kdo jim není srozumitelný, v odpovědi nebude.

Dobrá zpráva: co fungovalo pro vývojáře, funguje i pro agenty. Jen to musí být dotažené.

## Dokumentace je rozhraní

Dobré API se špatnou dokumentací je špatné API. Pro agenta to platí dvojnásob, protože se nemůže zeptat kolegy. Potřebuje krátký úvod, jak věci fungují, příklady a úplnou referenci endpointů, parametrů a chyb.

## Konzistentní názvy

Stejná věc má všude stejné jméno. Člověk si nekonzistenci domyslí, agent ji pochopí jako dvě různé věci.

## Chyby, podle kterých se dá jednat

Chybová hláška má říct, co se pokazilo a jak to opravit. Standardní HTTP kódy, jasný text. Agent podle ní zkusí krok znovu a správně, místo aby to vzdal.

## Obsah ve formátu pro stroje

- llms.txt v kořeni webu: krátké shrnutí, kdo jste a kde co najít.
- Markdown verze stránek: čistý text bez navigace a skriptů.
- Strukturovaná data (schema.org): kdo, co, kdy, pro koho.
- robots.txt, který AI crawlery pouští, a ochrana proti botům, která je omylem neblokuje.

Tenhle web to má všechno: https://www.honzasoukup.cz/llms.txt

## Rychlost

Agent pracuje v krocích a každý pomalý krok se násobí. Rychlost byla vždycky UX, u agentů rozhoduje o tom, jestli úkol vůbec dokončí.

## Testujte s agentem

Dřív jsem doporučoval dát API pěti vývojářům a sledovat, kde váhají. Dnes k tomu přidejte agenta: zadejte ChatGPT nebo Claude pět úkolů nad vaším webem či API a čtěte, kde se zasekne, co si vymyslí a kde to vzdá. Je to nejlevnější uživatelské testování, jaké existuje.
