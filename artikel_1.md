# Mijn HTML en CSS zijn chaos
In deze 3 artikelen leg ik uit hoe ik structuur heb leren aanbrengen in mijn websites. Ik leg dit uit door belangrijke leermomenten uit de minor uit te lichten. Het eerste artikel gaat over HTML

#### Help!
Voor dat ik begon aan de hva minor web-dev in februari van 2019 had ik nog nooit een regel HTML geschreven. Ik wist hoe het er uit zag maar wat er stond en waarom het er stond had ik geen idee van. Na 3 weken pielen zag mijn eerste site er zo uit. Er zat totaal geen logica in en niks wou op de plek gaan staan waar ik het wou hebben. Voor elke verandering maakte ik een nieuwe css selector en er staan een hele hoop dubbele stukken css code om er maar voor te zorgen dat alles consistent bleef. Het werkte, maar eigenlijk niet.

<details> <summary>HTML SNIPPET</summary>
	
```
<div data-grid="grid">
		<div data-bars="bar1">
		</div>
		<header>
			<div>
				<h1><span>MENU</span></h1>
				<p id="button">Day / Night</p>
				<a href="#platters">Platters</a>
				<a href="#eggs">Eggs</a>
			</div>
		</header>
		<main>
			<article>
				<div data-container="sticky">
					<div data-card="card">
						<h3>smoked fish</h3>
						<p><em>Serves 3 - 4 people</em> with cream cheese, onion, tomato, capers &amp; new potato salad and Russ &amp; daughters bread basket</p>
						<span>80</span>
					</div>
				</div>
			</article>
		</main>
```

</details>

<img src="https://i.gyazo.com/1e93783ee2d566ed42b35410d9999e19.png" width=900px></img>

Door de minor heen heb ik steeds een stukje bij geleerd over HTML en het structureren hiervan. Eigenlijk gaat het maar om één heel belangrijk begrip; semantiek.

### Semantiek
Semantiek in HTML betekend dat alle verschillende onderdeel, of tags, in je code waarde en betekenis hebben. Je wilt logische tags gebruiken voor de onderdelen op je site zodat je alle content kunt organizeren en je onderdelen kunt her gebruiken. Sinds HTML5 zijn er hiervoor tag voor content en voor containers. Containers gebruik je om vlakken en layout aan te leggen. Die layout vul je dan met content elementen. Een navigaties balk kan bijvoorbeeld bestaan uit een ```<nav>``` met daarin een paar ```<a>``` tags. De nav tag geeft aan dat het gaat om het navigatie gedeelte van de site en de content daarin zijn de linkjes naar verschillende delen van de site. 

Aangeven hoe belangrijk een stuk content op de site is, is ook belangrijk. Hiërarchische elementen zoals  ```<h1>``` ```<h2>```en ```<h3>``` zijn hiervoor. De meest belangrijke kop, waar de pagina over gaat, moet altijd een  ```<h1>``` tag krijgen. Hierna volgen de sub koppen en andere titels met  ```<h2>``` en  ```<h3>```. Door dit onderschijd heb je als lezer meteen overzicht. Andere content elementen zijn ```<p>``` tags voor een paragraaf en ```<img>``` voor afbeeldingen.

Qua layout zijn er sinds HTML5 dus allemaal nieuwe container tags. Waar in html4 overal ```<div>``` voor gebruikt werden zijn er nu bijvoorbeeld ```<header>```  ```<footer>```  ```<main>``` ```<nav>``` ```<article> ``` en ```<section>``` tags om te bouwen aan de layout. Waar al deze elementen geen waarde hebben zijn ze dus puur om de verschillende secties van de site te groeperen. 

Door al deze elementen goed toe te passen maak je het niet alleen voor jezelf als maken, of voor de gemiddelde bezoeker makkelijk en overzichtelijk. Ook zoekmachines en belangrijker nog, mensen met een handicap zijn enorm afhankelijk van een goed opgebouwde site. Voor hen is er geen hiërarchi of overzicht door een visuel overzicht dus kunnen ze alleen door goede semantiek weten waar ze zijn op een site en wat belangrijk is.

#### Conclusie
Volgens mij gaat de structuur in mijn sites al aardig de goede kant op. Als ik bovenstaand stuk code opnieuw zou schrijven zou ik dat op de volgende manier doen:

<details> <summary>HTML SNIPPET</summary>
	
```
<body>
	<nav>
		<h3>MENU</h3>
		<a href="#platters">Platters</a>
		<a href="#eggs">Eggs</a>
		<button>Day / Night</button>
	</nav>
	<main>
	  <section class="card">
			<h3>smoked fish</h3>
			<p><em>Serves 3 - 4 people</em> with cream cheese, onion, tomato, capers &amp; new potato salad and Russ &amp; daughters bread basket</p>
			<span>80</span>
		</section>
	</main>
</body>
```

</details>







