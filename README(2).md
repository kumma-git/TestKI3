# Fundstück-Scanner (Ein-Datei-Version)

In dieser Version stecken **Modell und Labels direkt im Code**
(`app.py`). Auf GitHub müssen daher nur zwei Dateien liegen:

- `app.py`
- `requirements.txt`

## Auf GitHub hochladen

1. Neues Repository erstellen.
2. `app.py` und `requirements.txt` hochladen.
3. Fertig.

## Auf Streamlit Cloud veröffentlichen

1. Auf [share.streamlit.io](https://share.streamlit.io) einloggen.
2. „New app" → das Repository auswählen.
3. Als „Main file path" `app.py` angeben.
4. „Deploy" klicken.

## Hinweis

`app.py` ist mit rund 3,2 MB deutlich größer als normaler Code, weil das
Keras-Modell als Base64-Text direkt eingebettet ist. Das ist technisch kein
Problem (GitHub erlaubt Dateien bis 100 MB), macht die Datei aber
unübersichtlich, falls du später am Code selbst etwas ändern willst.
Wenn du lieber Modell und Code getrennt hältst (übersichtlicher, Modell
lässt sich einfach austauschen), nimm die andere Version mit separaten
Dateien (`keras_model.h5` + `labels.txt` + `app.py`).
