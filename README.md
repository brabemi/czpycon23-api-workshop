# Moje první API ve Flasku

[PyCon CZ 23](https://cz.pycon.org/2023/program/workshops/20/), inspirováno pyworkingem [cojeapi](https://cojeapi.cz/)

Vyzkoušíme si vytvořit jednoduchou Flask aplikaci, která bude implementovat REST API a přijímat zprávy ve formátu JSON.

Výsledkem bude běžná CRUD aplikace s možností uložit a načíst stav z lokálního souboru.

Poslední část workshopu budeme věnovat diskuzi a nápadům, jak by aplikace šla rozšířit na základě obecných znalostí nebo na základě znalostí nabytých z ostatních přednášek v rámci konference.

## Vytvoření a aktivace venv

```
python3 -m venv venv
source venv/bin/activate
```

## Instalace závislostí

```
python -m pip install -r requirements.txt
```

## Spuštění
```
flask --app 09_api.py run
flask --app 09_api.py run --debug
```
## Co si naprogramujeme

Cílem je napsat si jednoduchou API službu. Služba umožní evidovat projekce na filmovém festivalu, kde každá projekce obsahuje:
- začátek
- délku
- název filmu
- krátký popisek

## Co budeme potřebovat znát

JSON: Něco jako slovník v Pythonu, ale funkční napříč mnoha dalšími teachnologiemi.

Ukázka
```json
{
  "description": "Popkulturní klasika no 2",
  "duration": 99,
  "name": "Rambo 2",
  "start_time": "2023-09-17 18:30:00.000"
}
```

Klient: Doplněk do prohlížeče Yet Another REST Client pro Chrome, zkušenější mohou použít rovněž curl nebo Postman.

## Soubory

### 01_api.py
Nejjednodušší možná verze API tzn. "hello world" ve Flasku.

### 02_api.py
Přidáváme kód který nefunguje a zkusíme si to opravit a použít `--debug`.

### 03_api.py
Ukáza toho jak lze pomocí URL předat do kódu různé parametry.

### 04_api.py
Ukáže jak lze do kódu předat různé metody HTTP.

### 05_api.py
Test toho jak pracovat s endpointy které mají růzmé metody HTTP a parametry.

### 06_api.py
Přidáváme CRUD operace pro naše API podle REST konvencí. První endpoint pro vypsání všech projekcí.

### 07_api.py
Přiidáváme pomocné fukce, které se použijí napříč celým API

### 08_api.py
Vytvoříme si ukázková data a následně i metodu pro vypsání projekce podle ID.

### 09_api.py
API rozšíříme o metody pro vytvoření, aktualizaci a smazání projekce.
