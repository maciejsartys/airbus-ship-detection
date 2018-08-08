.. quickstart:

Szybki start
============

Ogólne informacje odnośnie projektu. Zakładam, że uczestnicy znają Pythona w stopniu minimum podstawowym i posiadają przynajmniej ogólną wiedzę dotyczxącą zagadnień Machine Learning i Deep Learning. W toku prac przygotuję odpowiednie "bryki" dotyczące szczegółów implementacji sieci neuronowych i zasad ich działania. Różnice, plusy, minusy. 



Ważne linki
-----------

===============   =======================================================
Nazwa             URL
---------------   -------------------------------------------------------
GitHub            https://github.com/mdyzma/airbus-ship-detection.git
Slack             https://kagglepolska.slack.com/messages/CC4MR2S9G
Dokumentacja      https://airbus-ship-detection.readthedocs.io/en/latest/
===============   =======================================================



Terminy
-------

===============    ==================================
Start              **30. lipiec 2018**
Łączenie grup      **27. Wrzesień 2018**
Submisje           **27. Wrzesień 2018**
Koniec konkursu    **4. Październik 2018 23:59 UTC**
===============    ==================================



Nagrody
-------

Łączna pula nagród: **$60,000**

===================    =======
Pierwsza nagroda       $25,000
Druga nagroda          $15,000
Trzecia nagroda        $5,000
Najszybszy algorytm    $15,000
===================    =======



Wybrane zasady
--------------

1. Pięć submisji na dobę
2. Możliwość wyboru 2 do oceny finałowej.
3. Zakaz używania zewnętrznych zestawów danych (patrz dyskusja_), ale możliwość używania pre-trenowanych sieci pod warunkiem ich rejestracji na Forum.



Proponowane etapy i działania
-----------------------------

Większość skryptów zmieści się w pojedynczym notebooku, który zamieszczę na Platformie Colab od Google (ze względu na możliwość trenowania na GPU). Tam też wrzucę dane treningowe. Na początku testowe. Dodam, że każdy może robić próby sam na własnym koncie google colab używając niewielkiej, losowej próbki kilku tysięcy zdjęć (w zestawie treningowym jest ich 104 000). Proponuję więc już teraz nauczyć się obsługi colab i zobaczyć jak idzie uruchamianie GPU. Możemy się też umówić na sesję treningową, którą poprowadzę i każdy zaproszony będzie mógł zobaczyć jak to wygląda w praktyce.


    1. Ściągnięcie zestawu danych (każdy musi indywidualnie)
        - waga 26 GB
        - konto google airbus-kaggle-test
        - konto google airbus-kaggle-train

    2. Zaznajomienie z interfejsem i działaniem Google Colab
         - uruchamianie kodu pythona
         - używanie preinstalowanych bibliotek
         - akceleracja GPU

    3. Zadania koncepcyjne:
        - Losowanie próbki do testowania zmian obrazków (ostrość, kanały barw etc).  Trochę EDA i prawdopodobieństwa.
        - dobór rodzaju modyfikacji obrazków. Tutaj trochę teorii o kodowaniu kolorów, kanałach i sposobach ich analizy oraz modyfikacji
        - dobór odpowiedniej metody/metod ewaluacji. Trochę teorii o rodzajach sieci nuronowych i ich zastosowaniach
        - dobór pre-trenowanych algorytmów. Przedstawienie istniejących rozwiązań OpenSource.
    

    4. Zadania programistyczne:
        - Skrypt sprawdzający poprawność zdjęć (czy wszystkie są 768x768)
        - wprowadzenie do scikit-learn
        - Wprowadzenie do biblioteki KERAS
        - Generator danych
        - Modyfikacja danych(zdjęc)
        - Próba znanych pre-trenowanych sieci neuronowych i zmian danych na sub-próbie testowej (szybkość)
        - Ostateczne uformowanie etapów pracy w pipeline
        - Trening wszystkich danych treningowych na GPU Colab (potrzebne nowe konto, zestaw testowy ma  14.5GB)
        - Ewaluacja przyużyciu danych testowych (osobne konto z przeniesioną siecią neuronową)
        - Modyfikacje, prunning (opcjonalne) <- GOTO 6
        - Zapisanie modelu
        - Predykcja i utworzenie pliku do submisji


Każdy z tych etapów będzie wymagał jakiejś dyskusji (slack/hangout, ponieważ pisanie tekstu zajmuje więcej czasu, niż mówienie do mikrofonu). Do administracji możemy użyć trello z poziomu Slacka, lub tablicy githuba do zarządzania zadaniami. Ponieważ, to ja jestem pomysłodawcą, będę również koordynatorem wprowadzającym przedyskutowane zmiany, etapy na koncie projektu. jednak proponuję wyznaczyć kilka osób, które również będą mogły działać w projekcie (dodam je do grupy na GH) na wypadek mojej absencji (rodzina, dom, wakacje :-) )

Pozostałe sprawy organizacyjne
------------------------------

Generalnie możemy się umówić na codzienne spotkania na colab (10-15 minut max). Będziemy w miarę możliwości "symulować" metodologię scrum, ale dopasowaną do naszych potrzeb. Mamy już kanał na slack_, żeby móc się komunikować (jest możliwość dzwonienia do siebie, nie wiem jak z wieloosobowymi telekonferencjami). Jeżeli ktoś ma możliwości można też podczas sesji z colab używać hangouta, tam z pewnością można zapraszać wielu uczestników. Termin spotkań do ustalenia.

Kolejne rozdziały będą opisem tego jak co zrobić, lub zbiorem linków do przydatnych tutoriali i artykułów w sieci.

Przewiduję też sesje "na żywo" w colab, gdzie będziemy rozwiązywać problemy na bieżąco.


.. Linki

.. _zasady: https://www.kaggle.com/c/airbus-ship-detection/rules
.. _dyskusja: https://www.kaggle.com/c/airbus-ship-detection/discussion/62273
.. _Colab: https://colab.research.google.com
.. _slack: https://kagglepolska.slack.com/messages/CC4MR2S9G


