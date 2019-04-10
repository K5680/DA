## Teoriaa ja tekniikoita

*[Koneälyteoriaa suomeksi + hyvä englanti-suomi-machine learning -sanasto](https://tim.jyu.fi/view/kurssit/tie/tiep1000/tekoaly-mat/moniste)*

---


### Metodit



* **Regressioanalyysi (regression analysis)**

    Regressioanalyysi yrittää selittää muuttujaryhmän vaikutusta muuhun tutkittavaan muuttujaan.

    _Lineaarinen regressio_ on yleisin ennakoiva analyysi. Käytetään kuvailemaan dataa ja selittämään muuttujien yhteyksiä.
    Mitkä ovat henkilön arvioidut tulot?


    _Logistista regressioanalyysia_ käytetään silloin, kun selitettävä muuttuja voi saada vain kaksi arvoa. True/False, Pass/Fail...
    Mikä on lainan saamisen todennäköisyys? 


    _Pienimmän neliösumman keino (ordinary least squares, OLS):_ Etsitään käyrä, joka poikkeaa mahdollisimman vähän kahden muuttujan
    välistä yhteyttä kuvaavasta pistejoukosta (ääriarvotehtävä -> derivoidaan). 


    _Notebook-tutorial:_ 
    
    [nasan moottoridata/nasan_moottorien_elinikä.ipynb](../nasan_moottoridata)
    
    _Links:_
    
    [Video, logistinen regressioanalyysi](https://moniviestin.jyu.fi/vanhat/sosnet/sosnet5/5/2007-08-21.2314092629/view)
    
    [Video, pienimmän neliösumman keino](https://www.youtube.com/watch?v=qPUKBhHEmNI)  
    
    [Creating a Simple Linear Regression Machine Learning Model with scikit-learn
by Jonathan Wood](https://www.wintellect.com/creating-a-simple-linear-regression-machine-learning-model-with-scikit-learn/)
    
    
---


***Luokittelualgoritmit***


* **Päätöspuut (decision trees)**

    Prosessikaavio-tyyppinen algoritmi, jossa jokaisessa solmussa tehdään päätös, jokainen haara on valittu päätös ja 
    "lehti" kuvastaa tulosta. Polku juuresta lehteen = luokittelusäännöt. Voidaan myös kuvata joukkona assosiaatiosääntöjä.


    _Links:_

    [Päätösanalyysi](https://mycourses.aalto.fi/pluginfile.php/498011/mod_resource/content/5/L07-Paatosanalyysi.pdf)
    
    [Päätöspuun kasvattaminen](https://www.cs.helsinki.fi/group/joko/viikko4.pdf)



---

* **K:n lähimmän naapurin menetelmä (K-nearest neighbour)** 

    _luokittelu, regressio_
    
    Nnn-ulotteisessa avaruudessa oleville datapisteille etsitään K lähintä pistettä, ja se luokitellaan naapurien luokkien avulla. 
    Regressiossa keskiarvoa, ja moodia luokittelussa. 



    _Links:_ 
    
    [kNN wikipediassa](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm)
    
    [k:n lähimmän naapurin menetelmä](http://www.it.lut.fi/project/52105/thesishtml/node16.html)

---

* **Perseptroni (perceptron)**


    Algoritmi binääristen luokittelijoiden ohjattuun oppimiseen.
    
    [Video, MIT lecture: deep-learning, perceptron, loss optimization.](http://introtodeeplearning.com/)
    
    _Notebook-tutorial:_ 
    
    [nasan moottoridata/nasan_moottorien_elinikä.ipynb](../nasan_moottoridata)
    
    _Links:_

    [python perceptron](http://stamfordresearch.com/python-perceptron-re-visited/)  
    
    [Crash Course On Multi-Layer Perceptron Neural Networks](https://machinelearningmastery.com/neural-networks-crash-course/)
    
    
---


* **Tukivektorikone (SVM - support vector machine)**

    Luokittelee dataa etsimällä lineaarista hypertaso. Voidaan käyttää myös regressioanalyysiin (svr = support vector regression).
    
 
    _Links:_

    [Johdatus tekoälyn taustalla olevaan matematiikkaan](https://tim.jyu.fi/view/kurssit/tie/tiep1000/tekoaly-mat/moniste)

    [svm simple explanation](https://www.kdnuggets.com/2016/07/support-vector-machines-simple-explanation.html)
    
    [Video, SVM](https://www.youtube.com/watch?v=N1vOgolbjSc)
    
---


* **Naive Bayes (Naive Bayes)**

    Todennäköisyysluokittelu, perustuu Bayesin teoreemaan (esim. spam-suodatus)
    
 
    _Links:_

    [Naive Bayes Classification With Sklearn](https://blog.sicara.com/naive-bayes-classifier-sklearn-python-example-tips-42d100429e44)


---


***Muut***


* **Klusterointi (clustering)**

    Klusteroinnissa aineistosta pyritään löytämään ryhmiä, ja jakamaan alkiot ryhmiin niin, että alkiot kussakin ryhmässä ovat
    keskenään mahdollisimman samanlaisia, mutta alkiot eri ryhmässä mahdollisimman erilaisia keskenään. Luokittelussa pääsääntöisesti
    luokat on määritelty valmiiksi, klusteroinnissa ryhmät pyritään löytämään yhtäläisyyksien perusteella.

    _K-means:_ Tunnetuimpia klusterointimenetelmiä (iteratiivinen). Nopea ja helppo, mutta ei voi käsitellä 'dirty dataa' ja poikkeamia.

    ```
    1. Valitse satunnaiset alkiot klustereiden keskipisteiksi
    2. TOISTA
      3. Sijoita kukin aineiston alkio siihen klusteriin, jonka keskipiste on lähinnä
    4. Korvaa kunkin klusterin keskipiste klusterin alkioiden keskiarvovektorilla
    5. KUNNES (klustereiden keskipisteet eivät enää muutu)
    ```

    ([Klusterointimenetelmät. Tuononen, Marko.](https://cs.joensuu.fi/~mtuonon/Klusterointimenetelmat.pdf))


    _Notebook-tutorial:_ 
    
    [earthquake/earthquake.ipynb](../earthquake)
    
    _Links:_
        
    [K-means clustering in Python](http://stamfordresearch.com/k-means-clustering-in-python/)
    
    
---


* **Assosiaatioanalyysi/ostoskorianalyysi (association analysis/market basket analysis)**

    Pyrkimys löytää tuotteet, joita usein ostetaan joidenkin muiden tuotteiden kanssa. Tietoa voi hyödyntää
    esim. tuotteiden sijoittelussa (tätä ostaneet ostivat myös näitä...) 
    
    _Apriori_-algoritmi yleisin, jolla etsitään assosiaatiosääntöjä.


    _Notebook-tutorial:_ 
    
    [market_basket/marketbasket_analysis.ipynb](../miscellanous)


    
    _Links:_
    
    [Kehittynyt data-analytiikka vähittäiskaupan alalla](http://epublications.uef.fi/pub/urn_nbn_fi_uef-20160089/urn_nbn_fi_uef-20160089.pdf)
    
    [Ostoskorianalyysi vähittäiskaupan markkinoinnin tukena (Apriori s.31-32)](https://www.theseus.fi/bitstream/handle/10024/86733/Rasanen_Antti.pdf?sequence=1)

    _Python:_
    
    [Apriori Algorithm Python 3.0](http://adataanalyst.com/machine-learning/apriori-algorithm-python-3-0/)

    
---




* **Aikasarja-analyysi (Time series analysis)**

    Tunnistetaan ja mallinnetaan aikasarjan rakenne. Ennustetaan tulevia arvoja perustuen aikasarjaan.
    
    Pörssikurssit, valuuttakurssit, seuraavan kuukauden myynnin ennuste, tarvittavien varaosien tarve -ennuste (mm. Box-Jenkins metodi)
    
    _Notebook-tutorial:_

    [LAM-aikasarja-analyysi](../LAM)

    
    _Links:_

    [Aikasarja-analyysi (JYU)](https://koppa.jyu.fi/avoimet/hum/menetelmapolkuja/menetelmapolku/aineiston-analyysimenetelmat/aikasarja-analyysi)

---


* **Normalisointi**

    Tietokannan normalisoinnilla saadaan vaiheittain tietokannan rakenne paremmaksi, jotta tallennus ja tiedon haku on tehokasta. ([Tietokannan normalisointi, Wikipedia](https://fi.wikipedia.org/wiki/Tietokannan_normalisointi))

 
    _Links:_

    [Tietokannan normalisointi](https://support.microsoft.com/fi-fi/help/283878/description-of-the-database-normalization-basics)
    
    [What's the difference between normalization, standardization and regularization](https://www.quora.com/What-is-the-difference-between-normalization-standardization-and-regularization-for-data?share=1)
    

---




### Matematiikka

* **Keskiarvo (mean)**

---

* **Keskihajonta (standard deviation)**

    Mittaa sitä, kuinka paljon arvot poikkeavat keskiarvosta. Keskihajonta on varianssin neliöjuuri. 
    Etuna varianssiin nähden on tulkinnan helppous, sillä keskihajonnan asteikko vastaa mittausten asteikkoa.
    ([Hajontaluku, wikipedia](https://fi.wikipedia.org/wiki/Hajontaluku))
    
---

* **Varianssi (variance)**

    Keskihajonnan neliö. Varianssi ja keskihajonta kertovat, kuinka hajanaista data on. 
    Lähellä keskiarvoa keskihajonta on pieni. _Poikkeamat (outlier)_ lisäävät keskihajontaa.

---

* **Korrelaatio (correlation)**

    Kahden muuttujan välisen tilastollisen riippuvuuden mitta

    1 vahva positiivinen riippuvuus     
    -1 vahva negatiivinen riippuvuus        
    0 = ei riippuvuutta     


   
    _Links:_
        
    [Korrelaatio ja sen merkitsevyys](https://tilastoapu.wordpress.com/2011/11/01/10-korrelaatio-ja-sen-merkitsevyys/)
   
    
---

* **Mediaani (median)**

    järjestetyn joukon keskimmäinen alkio 

---

* **Kulmakerroin (slope)**

---

* **Kaltevuuskulma (gradient)**

---

* **Leikkauspiste (intercept)**

    Piste, jossa suora kohtaa akselin.

---

* **Kovarianssi (covariance)**

    Kuvaa, kuinka läheisesti muuttujat vaihtelevat yhdessä

---

* **Keskivirhe (standard error)**

    Keskivirhe tarkoittaa tilastotieteessä keskimääräistä virhettä ja sitä voidaan 
    käyttää mittaamaan tiettyä todennäköisyyttä vastaavaa luottamusväliä.
    [Wikipedia](https://fi.wikipedia.org/wiki/Keskivirhe)

---

* **Tilastollinen testaus (hypothesis testing)**

    Nollahypoteesi (null hypothesis) H0     
    Vaihtoehtohypoteesi (alternative hypothesis) HA     
    
---

* **Gradient descent**

    Suomessa gradientti, tai "kaltevuuden pienennys". Funktion tavoite on etsiä nopeimmin funktiota pienentävä suunta. 
    Käytetään kriittisten pisteiden etsimiseen.



--- 

### Tilastotiede


    
* Bayesiläinen tilastotiede

    frekventistisen (eli klassisen) tilastotieteen ohella tilastotieteen toinen suuri paradigma. 
        
* Premissi

    lähtökohta 
        
* Deduktio

    johtopäätös, deduktiivisessa päättelyssä tosi premisseistä seuraa väistämättä tosi johtopäätös  
        
* A priori

    ennen (analyyttisiä, välttämättömiä totuuksia) 
        
* A posteriori

    jälkeen. Edellyttää aistikokemuksen (synteettisiä / kontingentteja(sattuma)) 
        
    
    
