# Moje první API ve Flasku

[PyCon CZ 23](https://cz.pycon.org/2023/program/workshops/20/)

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

##
```
flask --app 09_api.py run
flask --app 09_api.py run --debug
```
