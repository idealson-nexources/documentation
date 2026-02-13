=============
ePOS printers
=============

ePOS printers are designed to work seamlessly with Point of Sale systems. Once connected, these
devices automatically share information, allowing for direct printing of tickets from the POS system
to the ePOS printer.

Configuration
=============

To use an ePos printer in Point of Sale:

#. :ref:`Access the POS settings <pos/use/settings>`.
#. Activate the :guilabel:`ePos Printer` feature.
#. Fill in the field with your ePos IP address.

.. image:: epos_printers/setting.png
   :alt: setting to enable the ePos printer feature

.. note::
   When the printer connects to a network, it automatically prints a ticket with its IP address.

Directly supported ePOS printers
================================

We strongly recommend using the **Epson TM-m30 i/ii/iii (Wi-Fi/Ethernet models only)**
model, which has been tested by us.

However, other Epson Wi-Fi/Ethernet models compatible with **ePoS Protocol** should also work.

Please keep in mind that the ePoS printer must be able to operate in HTTP mode.

ePOS printers with IoT system integration
=========================================

The following printers require an :doc:`IoT system </applications/general/iot/devices/printer>` to
be compatible with Odoo:

- Epson TM-T20 family (incompatible ePOS software)
- Epson TM-T88 family (incompatible ePOS software)
- Epson TM-U220 family (incompatible ePOS software)

.. important::
   - Epson printers using Wi-Fi/Ethernet connections and following the `EPOS SDK Javascript protocol
     <https://download4.epson.biz/sec_pubs/pos/reference_en/technology/epson_epos_sdk.html>`_ are
     compatible with Odoo **without** needing an :doc:`IoT system
     </applications/general/iot/devices/printer>`.
   - Thermal printers using ESC/POS are compatible **with** an :doc:`IoT system
     </applications/general/iot/devices/printer>`.
   - Epson printers using only USB connections are compatible **with** an :doc:`IoT system
     </applications/general/iot/devices/printer>`.
   - Epson printers that connect via Bluetooth are **not compatible**.

.. seealso::
   - :doc:`pos_lna`
   - :doc:`epos_ssc`
