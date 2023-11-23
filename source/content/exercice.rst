Exercices
=========

Exercice 1
----------

On donne la table ASCII:

.. container:: center

   .. image:: ../img/tableASCII.png
      :alt: image
      :align: center
      :width: 560

#. Que remarque-t-on dans la table ASCII en observant les lettres
   majuscules et les lettres minuscules ?

#. Donner les codes binaires des lettres A, a, M, m et W, w.

#. Quelle observation peut-on faire entre le codage binaire des
   majuscules et celui des minuscules?

.. _exercice-1:

Exercice 2
----------

Voici le code d'une page web html à copier coller dans un fichier avec l'extension ``html``.

.. literalinclude:: ../doc/ex_encodage_utf_iso_html.html
	:language: html

Ce fichier html est téléchargeable : :download:`fichier html<../doc/ex_encodage_utf_iso_html.html>`

Ouvrir ce fichier avec un navigateur et répondre aux questions posées.
	

.. _exercice-2:

Exercice 3
----------

Un caractère a comme point de code **U+005A**.

#. A quelle plage appartient ce point de code ?
#. Combien d'octets faut-il pour l'encoder en UTF-8 ?
#.	Ce caractère est-il un caractère de la table ASCII? Si oui, en déduire son encodage en binaire.

Exercice 4
----------

Le caractère de point de code **U+FFFD** appartient à la plage :math:`[U+0800 ;
U+FFFF]`. Ce caractère est donc encodé en UTF-8 sur trois octets.


#. Quel est la forme d'encodage de ce caractère en UTF-8 ?
#. Convertir en binaire le point de code de ce caractère.
#. En déduire l'encodage de ce caractère en UTF-8, c'est à dire tel qu'il est
   encodé en machine.
#. Convertir l'encodage binaire en hexadécimal.


Exercice 5
----------

Dans la langue française, on retrouve des ligatures, c’est à dire que certaines lettres sont collées l’une à l’autre. Par exemple, le o et le
e sont collés dans les mots nœud, œil et œuvre.

La ligature œ est apparue dans la table ISO 8859-15 avec le code hexadécimal BD.

Dans la norme Unicode, cette ligature a pour point de code **U+0153**.

On rappelle que le codage binaire en UTF-8 se fait en suivant les indications du tableau ci-dessous.

.. csv-table::
	:header: Plage, Ecriture binaire, Nombre de bits
	:file: ../csv/table_unicode.csv
	:delim: &

#. Combien faut-il d’octets pour coder la ligature **œ** en UTF-8
#. Après avoir converti le point de code en binaire, en déduire le codage binaire en UTF-8 de la ligature **œ**.
