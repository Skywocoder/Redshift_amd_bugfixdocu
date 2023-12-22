> [!NOTE]
> Aktuell noch in Bearbeitung, daher im Probleme & Lösungen nur wenig Inhalt


# Kurzer InfoGuide zu AMD Grafikkarten in Redshift
Dieser Guide ist rein aus Erfahrungen und wird teilweise erweitert wenn neue Erfahrungswerte dazukommen.
Redshift bietet aktuell nur kompletten Support für Nvidia Graffikarten, daher sind nicht alle AMD Karten kompatibel.

Um Komponenten in Redshift zu aktivieren folgen sie bitte der Anleitung im Moodle die von den Proffesoren berreitgestellt wird. [^3]

> [!NOTE]
> **NVIDIA USER: Grafikkarten unter 8GB VRAM werden laut Maxon nicht Unterstüzt, verwenden auf eigne "Gefahr"**

> [!NOTE]
> Ich, der Autor, hafte für keine schäden die durch Experiemente bzw instalation von Driver passiern! Dies ist jedeglich eine Basis für alle die die Probleme in mit den AMD GPU's in Redshift haben und eine Lösungsansatz brauchen. Die verwendung dieses Guides setzt vorraus das man ein wenig Grundverständis hat von seiner Hardware (Welche komponenten in seinem Gerät verbaut sind z.b.) bzw wie man googelt falls eine Frage nicht beantwortet wird. 

<details  {::options parse_block_html="true" /}>
 
  <summary>MAC OS USER!</summary> 
  
  Der Amd support ist etwas kompliztierter das dieser auch mit direkt mit der Version von Redshift zusammenhängt.

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

  > Radeon Pro Vega II / Vega II Du

  > Radeon Pro W5500X/W5700X
> 
  > Radeon RX 6800/6800 XT/6900 XT
> 
  > Radeon W6800X MPX
> 
  > Thunderbolt eGPUs [^4]

  > Radeon RX Vega 56/64
> 
  > Radeon Pro WX 9100
> 
  > Radeon VII
> 
  > Radeon RX 5500/5500 XT/5600 XT/5700/5700 XT
> 
  > Radeon W6800X MPX


   
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
>[!NOTE]
>Oftmals sind Driver oder ähnliches ein Problem. Zum Lösen bzw testen von Problemen sind programme wie HardwareInfo / HardwareMonitor nicht schlecht da es ihnen möglich sit schnell die aktuellen Driver auszulesen. Während meinem testesn hatte ich fast alle R24 compatiblen Versionen durchprobiert. Da Der AMD Support erst ab Mai/Juni 2022 da ist, können ältere Versionen ignoriert werden.

>[!WARNING]
>Unter keinen umständen ist der Hybrid Rendering "Button" in den Einstellungen anzuklicken wenn eine GPU und CPU ausgewählt sind. Das kann dazu führen das CineR24 nicht mehr funktuniert und sämtliche Render zu einem Bluescreen führen.

>[!NOTE]
>Da MacOS MacOS ist und ich keine möglichkeit habe mehrer Tausend Euro für einen Mac mit AMD Grafikkarte zu zahlen ist sind evnentuelle Probleme in MacOS hier nicht angeführt.

<details>
  <summary>Die Graffikarte wird nicht angezeigt!</summary>
  <br>
   + Keine kompatible Graffikarte --> überprüfe auf kompabilität
   + falscher Driver --> überpüfe ob der richtige Driver instaliert ist
    
   <br>
  
   > **TIP** Manche Redshift Versionen sind stabiler / laufen besser als andere. Falls ein Problem bestehend bleibt, teste eine andere Version. 
  <br>
</details>

<details>
  <summary>Redshift rendert nur über die CPU!</summary>
  <br>
   + keine Graffikkarte ausgewählt --> wähle eine Graffikarte aus ( Voreinstellungen -> Renderer -> rendern | Anleitung Prof.) [^3]
<br>
   
   
   > **INFO** Akutell ein bekannter Fehler ist das Redshift die CPU priotisiert, daher kann es dazu führen das die Grafikkarte nicht voll ausgelastet wird. 
<br>
</details>

<details>
  <summary>Meine CPU wird nur zu 10% ausgelastet!</summary>
    <br>
   + Problem in Redshift -> AMD Driver überprüfen bzw Redshift neuinstaliern
<br>
   
   > **INFO** Akutell ein bekannter Fehler ist das Redshift die CPU priotisiert, daher kann es dazu führen das die Grafikkarte nicht voll ausgelastet wird. 
   <br>

</details>


 



[^1]: Quelle: https://www.maxon.net/de/article/maxon-announces-redshift-support-for-amd-radeon-pro-graphics-on-windows / https://www.maxon.net/en/requirements/redshift-requirements
[^2]: https://www.amd.com/de/support
[^3]: Die Anleitung befindet sich in den Links die von den Proffesoren bereigestellt werden ab der Übung "erstes Rendern mittels Redshift ....." In der Regel befindet sich aber die Einstellung unter **Voreinstellungen -> Renderer -> rendern**
[^4]: Die Angegebene Thunderbolt eGPU hat klarerweise eine Nvidia oder Radeon Karte aus der List zu sein. Bei Nvidia ist darauf zu achten das diese unter MacOS vermutlich NICHT unterstützt sind. 
[^5]: https://redshift.maxon.net/landing benötigt Maxon Login!!




