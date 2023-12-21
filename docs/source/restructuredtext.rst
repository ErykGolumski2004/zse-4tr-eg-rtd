Składnia elementów dokumentu ReStructuredText.
==============================================

Nagłówki tekstowe (poziomy 1-4)
-------------------------------

Poziom 1:

.. code-block:: rst

   Nagłówek Poziomu I
   =================

Poziom 2:

.. code-block:: rst

   Nagłówek Poziomu II
   ------------------

Poziom 3:

.. code-block:: rst

   Nagłówek Poziomu III
   ^^^^^^^^^^^^^^^^^^^^

Poziom 4:

.. code-block:: rst
   
   Nagłówek Poziomu IV
   ******************

Akapit tekstowy (treść)
-----------------------

.. code-block:: rst

   To jest zwykły akapit tekstu.
      To jest podakapit głównego tekstu.

Wynik:

To jest zwykły akapit tekstu.
   To jest podakapit głównego tekstu.


Akapit informacyjny (Note, Tip)
-------------------------------

.. code-block:: rst

   .. note:: To jest akapit informacyjny, zawierający dodatkowe informacje.

   .. tip:: To jest akapit z poradą lub wskazówką.

Wynik:

.. note:: To jest akapit informacyjny, zawierający dodatkowe informacje.

.. tip:: To jest akapit z poradą lub wskazówką.

Fragment kodu (liniowy, blokowy)
--------------------------------

Liniowy:

.. code-block:: rst

   `fragment kodu`.

Wynik:

`fragment kodu`.

Blokowy:

.. code-block:: rst

   .. code-block:: python

      Print("Hello, World!");
      Print("Hello, World 2!")

Wynik:

.. code-block:: python

   Print("Hello, World!")


Odnośnik (lokalny RtD, zewnętrzny-inny serwis)
----------------------------------------------

Lokalny RtD: 

.. code-block:: rst

   Do pliku w tej samej dokumentacji (pliku) - :doc:`oautorze.rst`
   Do nagłówka w tym samym dokumencie (pliku) - :ref:`Odnośnik (lokalny RtD, zewnętrzny-inny serwis`
   Do nagłówka w innym dokumencie (pliku) - :ref:`Odnośnik (lokalny RtD, zewnętrzny-inny serwis) <restructuredtext.rst>`

Wynik:

   Do pliku w tej samej dokumentacji (pliku) - :doc:`oautorze.rst`
   Do nagłówka w tym samym dokumencie (pliku) - :ref:`Odnośnik (lokalny RtD, zewnętrzny-inny serwis`
   Do nagłówka w innym dokumencie (pliku) - :ref:`Odnośnik (lokalny RtD, zewnętrzny-inny serwis) <restructuredtext.rst>`

Zewnętrzny (inny serwis): 

.. code-block:: rst

   Przeczytaj więcej na stronie `Google <https://www.google.com>`_.

Wynik:

Przeczytaj więcej na stronie `Google <https://www.google.com>`_.

Listy (numerowana, wypunktowana, definicji)
-------------------------------------------

Lista Numerowana (ex.: “1.”, “1)”, “(1)”, “A.”, “a)”, “(A)”, “iv.”. “VI)”):

.. code-block:: rst

   1. Item 1
      a) Item 1a.
      b) Item 1b.
   2. a) Item 2a.
      b) Item 2b.

Wynik:

1. Item 1
   a) Item 1a.
   b) Item 1b.
2. a) Item 2a.
  b) Item 2b.

Lista Wypunktowana (ex. "*", "+", "-", "•", "‣", lub "⁃"):

.. code-block:: rst

   - Pierwszy element listy wypunktowanej.
   + Drugi element

Wynik:

- Pierwszy element listy wypunktowanej.
+ Drugi element

Lista Definicji:

.. code-block:: rst

   term 1
      Definition 1.
   term 2
      Definition 2, paragraph 1.
      Definition 2, paragraph 2.
   - definicja

Wynik:

term 1
   Definition 1.
term 2
   Definition 2, paragraph 1.
   Definition 2, paragraph 2.
  - definicja

Obraz (z alternatywnym tekstem oraz podpisem)
----------------------------------------------

.. code-block:: rst

   .. image:: /docs/unnamed.png
      :width: 300px
      :align: center
      :alt: Alternatywny tekst obrazka

      Podpis pod obrazkiem

Wynik:

.. image:: /docs/unnamed.png
   :width: 300px
   :align: center
   :alt: Alternatywny tekst obrazka

   Podpis pod obrazkiem

Tabela (jeżeli istnieje)
------------------------

.. code-block:: rst

   +------------+------------+
   | Kolumna 1  | Kolumna 2  |
   +============+============+
   | Wiersz 1   | Wiersz 1   |
   +------------+------------+
   | Wiersz 2   | Wiersz 2   |
   +------------+------------+

Wynik:

+------------+------------+
| Kolumna 1  | Kolumna 2  |
+============+============+
| Wiersz 1   | Wiersz 1   |
+------------+------------+
| Wiersz 2   | Wiersz 2   |
+------------+------------+
