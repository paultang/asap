PWM Dimmer 
================
PWM Dimmer(3M2P) works with ESP32-DevKitC board. 
You can use it to control at most 3 lights at same time.

* Power: Total 150W
* Input: DC 24V; 
* Output: Dimmable 24V
* WIFI: 802.n
* Output Terminal: G12-2 aviation connector

.. image:: ../image/3m2p.png

.. admonition:: Homespan code sample
    
    Setup control and status GPIO

    ::

        homeSpan.setControlPin(17); // sets control button
        homeSpan.setStatusPin(26); // sets LED Pin
    
    Setup three monochromatic lights GPIO  

    ::

        new DEV_DimmableLED(17)
        new DEV_DimmableLED(23) 
        new DEV_DimmableLED(25) 
