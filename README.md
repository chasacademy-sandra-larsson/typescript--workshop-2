
# Typescript #2: Mer av Typescript 
👋 Se föreläsningen i tisdags och i onsdags ✅ 

**Syftet med denna workshop:** Vi går vidare från grunderna i Typescript och utforskar:

* Interfaces vs Types
* Index signatures
* Enums
* Hämta från API med Typescript 
* Generics


### Setup med vanilla TS-projekt

Vi fortsätter jobba i vanilla TS med Node. Förutom övning 2 där vi kör vår tsc-kompilearade js i browsern.

```
npm init
npm install typescript ts-node --save-dev
npx tsc --init
npx tsc // bygg om .ts => .js
ts-node index.ts // kör ts-filen i node
```


### Bra att veta

Alla uppgifter + extrauppgifter är framåtsyftande mot provet i Typescript i v 44.

Förutom övningen finns även extrauppgifter på externa sidor. Gör dessa för att repetera, få djupare förståelse. För att relatera tll kommande prov anger jag G-nivå eller VG-nivå.

På provet kommer man få använda sig av Typescriptdokumentationen, så börja bli vän med den redan nu :-)

[https://www.typescriptlang.org/docs/](https://www.typescriptlang.org/docs/)

# 👩🏽‍💻 Övning 1: Interfaces 

G-nivå

**Din uppgift:**

Arbeta 2 och 2.


I denna uppgift ska ni själva konstruera ett exempel som använder sig av:

* Ett "bas" interface och minst ett annat interface som **extendar** interfacet i fråga
* Minst en property i interfacet ska använda en **enum**
* Ni använder en **funktion eller en class som tar in ett interfaces** som argument och använder det i funktioner/classes
* En output för minst en objektdata 

När ni är klara ska ni lista skillnaderna mellan Interface och types: 

**Vad kan interfaces gör men inte type:s och vice-versa?**

# 👩🏽‍💻 Övning 2: Hämta från API och visa i DOM:en 

G-nivå till VG-nivå

**Din uppgift:**

Arbeta 2 och 2.

* Välj valfritt API (exempelvis Pokemon, väderdata)
* Skriv en async-funktion där fetch används, samt att du typar funktionen enligt Typescript (Promise)
* Skapa ett interface (eller flera nestlade) som beskriver objektdatan som tas emot. 
* Visa den fetchade datan i DOM:en som minst en lista. Hur du gör det är valfritt, men tänk på hur du typar HTML-elementen. 
* Din kompilerade ts-fil ska alltsa vara länkad på html-sidans script-tagg:

```<script src="./dist/index.js"></script>```

# 👩🏽‍💻 Övning 3: Generics

Svara på frågan: Vad är generics? Vad är fördelen med att använda en generiska typer i en funktion/interface/type/class?

Börja läs i Typescriptdokumentation och leta även andra källor.
[https://www.typescriptlang.org/docs/handbook/2/generics.html#handbook-content
](https://www.typescriptlang.org/docs/handbook/2/generics.html#handbook-content)

Uppgifter: 

1. Skapa en funktion som använder generiska typer. Funktionen ska ta in en array av vilken typ som helst och returna arrayen i omvänd ordning.
2. Skapa en funktion som tar in två parametrar "key" och "value" som vardera är en generisk typ (inte samma!) och returnera objektet av properties "key" och "value"

 ```
 makePair("name", "sandra")
 makePair("age", 28)
 
 //Returns
 {
  "key": "name",
  "value": "sandra"
} 
{
  "key": "age",
  "value": 28
} 
```
3. Skapa ett interface "Box" med en generisk typ T. Interfaces ska ha ett property "item" av typen T. Skapa en funktion "unbox" som tar in interfacet Box och returnerar "item".

```
const stringBox: Box<string> = { item: "Hello, TypeScript!" };
console.log(unbox(stringBox)); // "Hello, TypeScript!"

```
4. Hur kan man göra så att en funktion med generiska typer inte tillåter alla typer utan endast exempelvis string eller number? 

# 🏃🏽‍♂️ Extrauppgifter

Välj och vraka efter eget tycke :-)


1. [https://www.totaltypescript.com/tutorials/beginners-typescript
  ](https://www.totaltypescript.com/tutorials/beginners-typescript) Uppgift 9-18 G-nivå
2. [https://typescript-exercises.github.io/](https://typescript-exercises.github.io/) Uppgift 5, 7-10 VG-nivå
3. [https://github.com/LearningTypeScript/projects](https://github.com/LearningTypeScript/projects) - Följer [denna O'really bok](https://www.oreilly.com/library/view/learning-typescript/9781098110321/?_gl=1*pv2bzi*_ga*MTgzNjg0Njk0Ny4xNjk1MDMwMDU5*_ga_092EL089CH*MTY5NTIxMjAxOS4yLjEuMTY5NTIxMjIzNS40MS4wLjA.), men du måste inte ha boken. Utgå från mapparna and "Functions", "Interfaces", "Generics". De delar in övningarna Appertizer (= G-nivå), Entrees (VG-nivå), Desserts (VG-nivå)
4. [Matt Pocock Generics Workshop ](https://github.com/total-typescript/typescript-generics-workshop)




# ✅ Redovisning:
* Du redovisar minst uppgiften för övningen. 
* ***Om du inte kan delta på workshopen, redovisar du ovanstående nästkommande workshop***







