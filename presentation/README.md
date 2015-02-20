
# CKAN Meetup @ CSC 20.2.2015 | Avoindata.fi

Jari Voutilainen [@Zharktas](https://twitter.com/Zharktas) | [@GoforeOy](https://twitter.com/GoforeOy)

---

## Agenda

* Avoindata.fi
* Kuulumiset edellisen CKAN meetupin jälkeen
* Vuoden 2015 suunnitelmat

---

## Avoindata.fi

* Muodostaa käsitteen Yhteentoimivuuspalvelut
* Koostuu kahdesta palvelusta: avoimen datan metakatalogista ja yhteentoimivuuden kuvauksista.
* Palvelun on tilannut Valtiovarainministeriö, tuottanut Valtori ja toteuttanut Gofore.

--

## Yhteentoimivuuspalvelut

* Näkymä kansalliseen avoimeen dataan ja yhteentoimivuutta edistäviin työkaluihin ja ohjeisiin.
* Alustoina rinnakkain olevat Drupal ja CKAN.
* Suurin osa työstä keskittyy CKAN:n kustomointiin.

--

## Avoimuus

* Palvelu on monikielinen ja responsiivinen.
* Avoin kehitysmalli: lähdekoodit on saatavilla [Githubista](https://github.com/yhteentoimivuuspalvelut), [beta.avoindata.fi](http://beta.avoindata.fi/) on avoin testausympäristö, isommista muutoksista tiedotetaan somessa ja palvelun uutisissa.

--

## Tekniikat ja menetelmät

* Alustoina uusin CKAN (2.2.1) ja Drupal (7.34).
* Bugiraportteja ja korjauksia tehty CKAN:n coreen.
* Organisaatiohierarkiat
* Tietoaineiston metatietoja laajennettu useilla tietokentillä ja monikielisyydellä.
* Palveluun harvestoidaan HRI:n aineistot ja Paikkatietohakemistosta avoindata.fi:lle tägätyt.

--

* Kahden viikon sprintit (scrum), tuotanto päivitetään aina sprintin päätteeksi.
* Palvelu hostataan AWS:ssä Goforen ylläpitämänä.
* Päivitykset hoidetaan *Ansible*-konfiguraationhallinnalla
* Asennus on automatisoitu, myös virtuaalikoneissa oleviin kehitysympäristöihin.

--

* Kehitys tapahtuu Virtualbox virtuaalikoneessa Vagrantin avulla.
* Vagrant lataa Ubuntu 12.04 virtuaalikoneen, johon palvelu asennetaan ansiblen avulla.
* Ympäristö on testattu Ubuntu 12.04/14.04 ja Windows 7/8.1 käyttöjärjestelmissä.
* Tuotanto ja beta päivitetään AWS:ssä samalla ansible provisioinilla kuin kehitysympäristöt.

---

# Kuulumiset edellisen meetupin jälkeen

* Palvelu julkastiin 15.9., vähän ennen edellistä meetuppia.
* Julkaisun jälkeen asiakkaan tilaamat resurssit on käytännössä olleet 1 henkilö.
* Joten palvelu on pitkälti ollut pienkehityksessä.

--

* Suurin osa ajasta menee ylläpitoon: bugeihin, ylläpitäjille tehtyihin käyttöliittymiin, yhteentoimivuus -aineistojen paranteluun.
* Näkyvimpänä muutoksena on ollut uusi modernimpi ulkoasu, jota kehitetään myös jatkossa.
* Palvelutietovarannon poistuessa suunnitelmista, siihen liittyvät toiminnallisuudet poistettiin betasta ja organisaatio mallia yksinkertaistettiin.

--

* Tietoaineistoihin on lisätty "Liittyvät mediat", jotka ovat visualisointeja, sovelluksia, ideoita yms. Näitä voi kuka tahansa rekisteröitynyt lisätä ja organisaation ylläpitäjällä on vastuu moderoida ne tarvittaessa.
* Pienempinä muutoksina paremmat organisaatiolistaukset, alustava 5-portainen laatuluokitus, harvestereiden vikatoleranssin parantamista yms.

---

# Vuosi 2015

* Asiakas tilannut lisäresursseja, joten palveluun on tulossa parannuksia.
* Tietoaineistojen ja organisaatioiden kommentointi, voi esimerkiksi käyttää tietopyyntöihin.
* 5-portaisen laatuluokituksen parantelut, nykyinen toteutus melko yksinkertainen
* Käytettävyysparannukset, mm. etusivusta tehdään paremmin palvelua palveleva.
* Tietoaineistokohtaiset analyyttiikkatiedot.

--

* Teknisiä parannuksia.
* CKANin päivitys piakkoin tulevaan 2.3:een.
* Tietopyynnöille ehkä oma toiminnallisuus.
* Harvesteri integraatioita parannetaan.

---

# Kysyttävää ?
