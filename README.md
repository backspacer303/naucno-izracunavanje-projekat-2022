# Simbolička Furijeova transformacija u klasifikaciji vremenskih serija

## Kratak opis projekta
Simbolička Furijeova transformacija (SFA) je način za poređenje vremenskih serija. Ideja je da se vremenske serije se pretvaraju u vektore koji se onda lakše porede zbog manje dimenzionalnosti. Vremenska serija se transformiše u vektor dužine m tako što se nalazi prvih m Furijeovih koeficijenata. SFA je u projektu korišćen kao sredstvo za agregaciju. Početni problem podataka je što nisu iste granularnosti. SFA je onda korišćen da se podaci svedu na dnevnu granularnost.

Poenta ovog rada je da se podaci o Sunčevom zračenju koriste za predikciju početka poplava u Evropi.

## Podaci
Rad koristi podatke koji su rezultati merenja Sunčevog zračenja.  Podaci su preuzeti sa sajta https://sohoftp.nascom.nasa.gov/sdb/goes/ace/daily/ koji su prosledile kolege sa Geografskog Instituta "Jovan Cvijić", Srpska akademija nauka i umetnosti. Podaci o poplavama su uzeti većinom sa sajta kaggle: https://www.kaggle.com/datasets/tomkowski/european-past-floods?resource=download. Deo podataka o poplavama je dobijen sa Geografskog Instituta "Jovan Cvijić".

Svi podaci zajedno se mogu preuzeti [ovde](https://drive.google.com/file/d/1Kop0320shQJ_uoGm7vde3EAeEHcvFVoi/view?usp=sharing).

## Literatura
- Projekat prati koncepte iz naučnog rada *"A Symbolic Fourier Approximation and Index for
Similarity Search in High Dimensional Datasets"*, Patrick Schäfer, Mikael Högqvist:

  - https://openproceedings.org/2012/conf/edbt/SchaferH12.pdf

## Podešavanje okruženja

Paketi potrebni za pokretanje projekta:

- `pyts` paket za obradu i klasifikaciju vremenskih serija 
    
    ```bash
    pip install pyts
    ## ili
    conda install -c conda-forge pyts
    ```
- `pygtrie` paket korišćen za formiranje sufiksnog stabla
  ```
  pip install pygtrie
  ```
- `numpy`
  ```bash
  pip install numpy
  ## ili
  conda install numpy
  ``` 
- `pandas`
  ```bash
  pip install pandas
  ## ili
  conda install pandas
  ```
- `sklearn`
  ```
  pip install scikit-learn
  ```
- `matplotlib`
  ```bash
  pip install matplotlib
  ## ili
  conda install matplotlib
  ```
- `altair` paket korišćen za vizelizaciju
  ```bash
  pip install altair
  ## ili
  conda install -c conda-forge altair
  ```
- `nltk` paket korišćen samo za edit rastojanje (Levenshtein-ovo rastojanje)
  ```
  pip install nltk
  ```

## Članovi tima
Aleksandra Ružić 1044/2021
- GitHub: https://github.com/AleksandraRuzic

Nikola Perić 1096/2021
- GitHub: https://github.com/backspacer303