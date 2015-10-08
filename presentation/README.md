
# Open Finland Challenge Meetup @ Gofore 8.10.2015 | Avoindata.fi

Jari Voutilainen [@Zharktas](https://twitter.com/Zharktas) | [@GoforeOy](https://twitter.com/GoforeOy)

---

## Agenda

* Avoindata.fi
* Kesän kehitys
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

---

# Kesän kehitys

* Uusia ominaisuuksia:
  * Google analytics visualisoinnit tietoaineistoissa ja aineistolinkeissä.
  * Organisaatioille voi lähettää tietopyyntöjä
  * Etusivu uudistettiin
  * Tietoaineistoja voi kommentoida

--

* CKAN päivitettiin keväällä 2.3:een.
* Kesälomien aikaan tehtiin teknistä ylläpitoa.

---

# Suunnitelmissa olevat isommat asiat

* Tiedon avaajan opas
* AWS arkkitehtuurin uudistus
  * Varautuminen mahdolliseen datan hostaukseen.
* CKAN päivitetään 2.4:ään.
* Finto integraatio

--

* Uusi tietomalli
  * ckanext-scheming, ckanext-fluent
  * rajapinta tuottaa järkevämmän vastauksen
  * Samalla uudistetaan tietojen syöttölomakkeet

---

# Open Finland Challenge

* Avoindata.fi currently harvests datasets from hri.fi and paikkatietohakemisto.fi
* Harvesters are implemented in [ckanext-harvest](https://github.com/ckan/ckanext-harvest) extension
* Extension provides [CKAN harvester](https://github.com/ckan/ckanext-harvest/blob/master/ckanext/harvest/harvesters/ckanharvester.py) which is used to harvest hri datasets.
* Paikkatietohakemisto's datasets are harvested using [spatial csw harvester](https://github.com/ckan/ckanext-spatial/blob/master/ckanext/spatial/harvesters/csw.py).
* Current modified harvesters be found from [Github](https://github.com/yhteentoimivuuspalvelut/ytp/tree/master/modules/ckanext-ytp-main/ckanext/ytp/organizations/harvesters)

--

## Requirements

* Possible data source must have restish urls.
* Implemententation should be based on [base harvester](https://github.com/ckan/ckanext-harvest/blob/master/ckanext/harvest/harvesters/base.py)
* Implementation should be provided through [Github Pull Request](https://github.com/yhteentoimivuuspalvelut/ytp/pulls)
* All problems with dev environments should be reported through Github issues.
* If the implementation is decent enough, avoindata.fi devs will get permissions to harvest the data and install the harvester.
