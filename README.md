# Kurzer Guide zu AMD Grafikkarten in Redshift
Dieser Guide ist rein aus Erfahrungen und wird teilweise erweitert wenn neue Erfahrungswerte dazukommen.
Redshift bietet aktuell nur kompletten Support für Nvidia Graffikarten, daher sind nicht alle AMD Karten kompatibel.

**NVIDIA USER: Grafikkarten under 8GB VRAM nicht unterstützt/teilweise unterstützt**

<details>
  <summary>MAC OS USER!</summary>
    ### Mac-User insert
      Der Amd support ist etwas kompliztierter das dieser auch mit direkt mit der Version von Redshift             zusammenhängt.

    Grundsätzlich ist folgende Liste unterstützt: 

    **MacBook Pro**

    > Radeon Pro Vega 16/20
    > Radeon Pro 5500M/5600M

    **iMac**

    > Radeon Pro Vega 48
    > Radeon Pro 5500 XT/5700/5700 XT

    **iMac Pro**

    > Radeon Pro Vega 56/64

    **MacPro**

    > Radeon Pro Vega II / Vega II Duo
    > Radeon Pro W5500X/W5700X
    > Radeon RX 6800/6800 XT/6900 XT
    > Radeon W6800X MPX
    > Thunderbolt eGPUs

    > Radeon RX Vega 56/64
    > Radeon Pro WX 9100
    > Radeon VII
    > Radeon RX 5500/5500 XT/5600 XT/5700/5700 XT
    > Radeon RX 6800/6800 XT/6900 XT
    > Radeon W6800X MPX

    Die Angegebene Thunderbolt eGPU hat klarerweise eine Nvidia oder Radeon Karte aus der List zu sein. Bei Nvidia ist        darauf zu achten das diese unter MacOS vermutlich NICHT unterstützt sind. 
</details>


## Welche AMD Grafikkarten sind kompatibel?
Aktuell ist die verwendung von AMD Karten nur duch eine kombination aus Hardware und Software möglich.
Grundsätzlich ist es nicht möglich AMD Grafikkarten einzusetzen die nicht mit AMD RADEON PRO driver verwenden können einzusetzen. 

  Die Liste der unterstützen Graffikkarten findet man auf der Hardwareinfoseite von Redshift [^1]: 
  > Radeon PRO W7900, W7800

  > Radeon PRO W6800, W6600

  > Radeon VII (beide Variationen unterstützt)

  > Radeon W5700

  > Radeon RX 7950 XTX, RX7950 XT, RX7900

  > Radeon RX6950, RX6700 XT, RX6600

  > Radeon RX5700 XT

  Damit diese Graffikkarten unterstützt werden sind die AMD RADEON PRO driver [^2]







[^1]: Quelle: https://www.maxon.net/de/article/maxon-announces-redshift-support-for-amd-radeon-pro-graphics-on-windows / https://www.maxon.net/en/requirements/redshift-requirements
[^2]: https://www.amd.com/de/support
