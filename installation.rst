.. _installation:

Installation
============

Magento 2
-----------

Magento Marketplace
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Falls Sie das Modul über Magento Marketplace gekauft haben, können Sie es bequem über den *Component Manager* von Magento 2 installieren. Gehen Sie hierzu im Backend auf :menuselection:`System --> Web Setup Wizard` 

.. image:: /images/install-setup-wizard.png

Wählen Sie den *Component Manager* an, um Ihre Magento Installation zu verwalten.

.. image:: /images/install-setup.png

Um Module installieren zu können müssen Sie mit Ihrem Marketplace Konto verbunden sein.

.. image:: /images/install-component-manager-loggedout.png

Loggen Sie sich hierzu nun mit Ihrem Magento Marketplace Account in den *Component Manager* ein. Sie finden die *Access Keys* in Ihrem Marketplace Account unter `My Access Keys <https://marketplace.magento.com/customer/accessKeys/list/>`_.

.. image:: /images/install-marketplace-login.png

Sobald Sie eingeloggt sind und synchronisieren Sie den *Component Manager* mit Ihrer Magento Installation durch Klick auf **Sync**. Klicken Sie nun auf **Install** um die zu aktualisierenden Module auszuwählen.

.. image:: /images/install-component-manager-loggedin.png

Sie sehen eine Übersicht über alle Module zu denen neue Versionen vorliegen. Wählen Sie die gekaufte Extension aus und klicken Sie nochmals **Install**.

.. image:: /images/install-component-manager-install.png

Das Modul wird nun installiert und steht Ihnen zur Verfügung.

manuelle Installation / FTP
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Laden Sie die gekaufte Extension aus Ihrem Kunden-Account herunter
* Entpacken Sie die Extension in ein temporäres Verzeichnis
* Laden Sie die Extension in `app/code` in Ihrer Magento Installation
* Aktualisieren Sie den Cache
* Führen Sie das folgende Kommando auf der Kommandozeile aus:

.. code-block:: bash
	
	$ php bin/magento setup:upgrade

* Loggen Sie sich aus dem Magento Admin Panel aus, und wieder ein
* Das Modul steht Ihnen nun zur Verfügung

Composer Installation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Fügen Sie das Magento Composer Repository zu Ihrem Projekt hinzu, falls noch nicht vorhanden: 

.. code-block:: bash

	$ composer.phar config http-basic.repo.magento.com <public_key> <private_key>

* Installieren Sie das gekaufte Modul mit dem entprecheden Module Key:

.. code-block:: bash

	$ compose.phar require netzkollektiv/my-bought-module
	$ compose.phar update

* Aktualisieren Sie den Cache und Upgraden Sie Magento:

.. code-block:: bash

	$ php bin/magento cache:clean
	$ php bin/magento setup:upgrade

Magento 1
-----------

Magento Connect / Downloader
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Gehen Sie im Magento Backend auf :menuselection:`System --> Konfiguration --> Magento Connect --> Magento Connect Manager`

.. image:: /images/m1-connect-menu.png

Loggen Sie sich nochmal mit Ihren Backend-Zugangsdaten ein:

.. image:: /images/m1-connect-login.png

Laden Sie das über unseren Store zur Verfügung gestellt tgz-Archiv im Manager hoch.

.. image:: /images/m1-connect-upload.png

Das Modul steht Ihnen nun zur Verfügung.

manuelle Installation / FTP
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Laden Sie die gekaufte Extension aus Ihrem Kunden-Account herunter
* Entpacken Sie die Extension in ein temporäres Verzeichnis
* Laden Sie die Extension in die Struktur Ihrer Magento Installation
* Aktualisieren Sie den Cache
* Loggen Sie sich aus dem Magento Admin Panel aus, und wieder ein
* Das Modul steht Ihnen nun zur Verfügung

