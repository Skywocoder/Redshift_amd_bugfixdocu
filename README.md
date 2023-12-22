# Kurzer Guide zu AMD Grafikkarten in Redshift
Dieser Guide ist rein aus Erfahrungen und wird teilweise erweitert wenn neue Erfahrungswerte dazukommen.
Redshift bietet aktuell nur kompletten Support für Nvidia Graffikarten, daher sind nicht alle AMD Karten kompatibel.

Um Komponenten in Redshift zu aktivieren folgen sie bitte der Anleitung im Moodle die von den Proffesoren berreitgestellt wird. [^3]

> [!NOTE]
> **NVIDIA USER: Grafikkarten under 8GB VRAM nicht unterstützt/teilweise unterstützt**

<details>
  <summary>MAC OS USER!</summary>
    Mac-User insert
      Der Amd support ist etwas kompliztierter das dieser auch mit direkt mit der Version von Redshift                 zusammenhängt.

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

    > [!CAUTION]
    > Die Angegebene Thunderbolt eGPU hat klarerweise eine Nvidia oder Radeon Karte aus der List zu sein. Bei Nvidia ist darauf zu achten das diese unter MacOS vermutlich NICHT unterstützt sind. 
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

  Damit diese Graffikkarten unterstützt werden sind die AMD RADEON PRO driver [^2] benötigt:

  > AMD RADEON PRO 22 Q4 oder neuer

  Der normale AMD Radeon Driver wird von Radeon nicht unterstützt. 

  **ACHTUNG!** Der Driver updated sich unter umständen auf einen normalen Driver, was dazu führen kann das die     Grafikkarte nicht mehr von Redshift erkannt wird.
  
## Bekannte Probleme & Lösungen
<details>
  <summary>Die Graffikarte wird nicht angezeigt!</summary>
    + Keine kompatible Graffikarte --> überprüfe auf kompabilität
    + falscher Driver --> überpüfe ob der richtige Driver instaliert ist
    
    
    > [!TIP]
    > Manche Redshift Versionen sind stabiler / laufen besser als andere. Falls ein Problem bestehend bleibt, teste eine andere Version. 
  
</details>

<details>
  <summary>Redshift rendert nur über die CPU!</summary>
  + keine Graffikkarte ausgewählt --> wähle eine Graffikarte aus ( Voreinstellungen -> Renderer -> rendern | Anleitung Prof.) [^3]

  > [!NOTE]
  > Akutell ein bekannter Fehler ist das Redshift die CPU priotisiert, daher kann es dazu führen das die Grafikkarte nicht voll ausgelastet wird. 

</details>

<details>
  <summary>Meine CPU wird nur zu 10% ausgelastet!</summary>
  + Problem in Redshift 

  > [!NOTE]
  > Akutell ein bekannter Fehler ist das Redshift die CPU priotisiert, daher kann es dazu führen das die Grafikkarte nicht voll ausgelastet wird. 

</details>
  






[^1]: Quelle: https://www.maxon.net/de/article/maxon-announces-redshift-support-for-amd-radeon-pro-graphics-on-windows / https://www.maxon.net/en/requirements/redshift-requirements
[^2]: https://www.amd.com/de/support
[^3]: Die Anleitung befindet sich in den Links die von den Proffesoren bereigestellt werden ab der Übung "erstes Rendern mittels Redshift ....." In der Regel befindet sich aber die Einstellung unter **Voreinstellungen -> Renderer -> rendern**
