# Multilingual Online Translator

This application provides a service for receiving the translation data from online web service https://context.reverso.net/translation/

The languages that Multilingual Online Translator app can support are:
- Arabic
- German
- English
- Spanish
- French
- Hebrew
- Japanese
- Dutch
- Polish
- Portuguese
- Romanian
- Russian
- Turkish

____

### Requirements
- Python 3.7+
- Beautiful Soup 4
____
### Installing
1\. Clone the repository
```
    git clone https://github.com/AnnaKatunina/Multilingual_Online_Translator.git
```
2\. Create and activate virtualenv
```
    python -m venv venv
    source venv/bin/activate (for Linux/macOS) or venv\Scripts\activate (for Windows)
```
3\. Install packages from requirements.txt
```
    pip install -r requirements.txt
```
____
### Usage
Use command-line interface.

In the command line input a language which you want to translate from, a language you want translate to, and the word you want to translate.

As a result terminal will display 5 words and 5 example sentences.

Example:
> python translator.py english french hello
```
French Translations:
bonjour
allô
ohé
coucou
salut
 
French Examples:
Well, hello, freedom fighters.:
Et bien, bonjour combattants de la liberté.
 
Goodbye England and hello the Netherlands...:
Au revoir l'Angleterre et bonjour les Pays-Bas...
 
Yes, hello. Jackson speaking.:
Oui, allô, Jackson à l'appareil.
 
Hello, hello, hello, hello.:
Allô, allô, allô, allô.

And began appearing hello kitty games online.:
Et a commencé à apparaître bonjour Kitty jeux en ligne.
```
____
The second feature of this app is translation to all languages at once.

Instead of language to be translated input “all”.

As a result terminal will display one example word and one example sentence of each supported language.

Example:
> python translator.py english all hello
``` 
German Translations:
hallo
 
German Example:
We agreedellen wolf is innocent. hello.:
Wir waren einverstanden damit, dass Wolf unschuldig ist. Hallo.
 
 
Spanish Translations:
hola
 
Spanish Example:
Well, hello, Miss Anchor-liar.:
Bien, hola, señorita presentadora de mentiras.
 
 
French Translations:
bonjour
 
French Example:
Well, hello, freedom fighters.:
Et bien, bonjour combattants de la liberté.
 
 
Dutch Translations:
dag
 
Dutch Example:
That was kind of our funny hello.:
Dat vond we een grappige begroeting.
 
 
Polish Translations:
cześć
 
Polish Example:
I guess it's... goodbye car insurance, hello city bus.:
I domyślam się, że to jest... do widzenia ubezpieczenie samochodu, cześć autobus miejski.
 
 
Portuguese Translations:
olá
 
Portuguese Example:
That was my last kiss hello.:
Pois eu garanto que aquele foi o meu último beijo de olá.
 
 
Romanian Translations:
salut
 
Romanian Example:
Well, hello, professor Culbertson.:
Ei bine, salut, profesor universitar Culbertson.
 
 
Russian Translations:
привет
 
Russian Example:
Why, hello, there, Admiral.:
А, Адмирал, привет, что здесь делаешь.
 
 
Turkish Translations:
selam
 
Turkish Example:
So now little Sabina says hello.:
Velhasıl minik Sabina size selam söylüyor.
```
____
All results are saved in the file which is named as the word in the input.

In case of requests for a non-existent words, unsupported languages or internet connection errors the app raises exceptions such as:
```
Sorry, the program doesn't support this language
Sorry, unable to find this word
Something wrong with your internet connection
```