.. _de-software-installation:


=====================
Software Installation
=====================

Installing the system is fairly straight forward. You need to start with a `Raspberry-PI board that is up and running <https://www.raspberrypi.com/software/operating-systems/>`_ with ssh connection.
Different versions of software can be found `here <https://drive.google.com/drive/folders/1wMIw5VSW4CdIxMXIFMeq0AyuZBDIfFaH?usp=sharing>`_ 



|
.. youtube:: https://www.youtube.com/watch?v=cvQgMcnM7NA
|





Steps
=====

Open `Drone-Engage WebSite <https://www.droneengage.com>`_ and select **"Download Binaries"**.
|
Download the appropriate binary for your board and version.
|
Copy files to youe home folder in the board.
|

.. code-block:: bh

   scp ./drone_engane_RPI-Zero_v1.0.1.zip  pi@raspberry_pi_ip_address:.
|
Execute the following commands:
    
.. code-block:: bh

   ssh pi@raspberry_pi_ip_address

.. code-block:: bh

   unzip ./drone_engane_RPI-Zero_v1.0.1.zip
|
It will extract a folder and a file script.
|

.. code-block:: bh

   chmod +x ./install_droneengage.sh

.. code-block:: bh

   ./install_droneengage.sh
|
Update your account in file **./drone_engage/de_comm/config.module.json**

.. code-block:: bh

   nano ./drone_engage/de_comm/config.module.json 
|
Update your connection to Flight Controller in file **./drone_engage/de_mavlink/config.module.json**
   
.. code-block:: bh

   nano ./drone_engage/de_mavlink/config.module.json






   


