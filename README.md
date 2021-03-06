# Under conctruction...

# Real-time object detection with YOLO 3 (Keras)

Python-Framework zur Erkennung und Lokalisierung von Objekten in Bildern und Videostreams in Echtzeit. Das Framework basiert auf der [YOLO 3](notebook/YOLOv3.pdf) Implementierung (https://github.com/experiencor/keras-yolo3) von (https://github.com/experiencor).

Das Framework wurde so angepasst, dass ein und derselbe Sorce-Code sowohl lokal auf einem Windows 10 Rechner (mit GPU und ausreichend RAM) als auch mit der Deep Learning Platform "[FloydHub](https://www.floydhub.com/)" (preisgünstige Alternative zu Google Cloud Platform, Amazon AWS, ect.) ausgeführt werden kann. Da es sich hierbei um ein Linux-basiertes System handelt, sind einige Dinge zu beachten, wie z.B. die konsequente Beachtung von Groß-/Kleinschreibung und Verwendung von Forward-Slashes für Verzeichnis-, Datei- und Pfadnamen.

Die Struktur wurde so aufgebaut, dass die verschiedenen Modelle voneinander separiert sind und dass es leicht möglich ist weitere Modelle hinzuzufügen.

## YOLO (You only look once)
Im Vergleich zu anderen Methoden wie [SSD](https://arxiv.org/abs/1512.02325), [DSSD](https://arxiv.org/abs/1701.06659), [R-FCN](https://arxiv.org/abs/1605.06409), [RetinaNet](https://arxiv.org/abs/1708.02002) , ect. arbeitet [YOLO 3](notebook/YOLOv3.pdf) exterm schnell bei hoher Präzision (siehe https://pjreddie.com/darknet/yolo), daher ist [YOLO 3](notebook/YOLOv3.pdf) sehr gut für die Objekterkennung in Echtzeit geeignet. Während für das Training eine entsprechend gute GPU mit ausreichend Speicher benötigt wird, kann die Objekterkennung sogar auf weniger performanten CPUs wie beispielsweise einem [Raspberry PI 3](https://de.wikipedia.org/wiki/Raspberry_Pi) ausgeführt werden.

Hier einige Artikel über die Architektur und Arbeitsweise von YOLO:
- https://medium.com/jonathan_hui/real-time-object-detection-with-yolo-yolov2-28b1b93e2088
- https://blog.paperspace.com/how-to-implement-a-yolo-object-detector-in-pytorch/

## Anwendungsbeispiele:

#### Erkennung und Lokalisierung von Fahrzeugen, Verkehrszeichen und Personen in Echtzeit

[![](https://img.youtube.com/vi/MiJpW9fhUdw/0.jpg)](https://www.youtube.com/watch?v=MiJpW9fhUdw)

#### Erkennung von Waschbären in Echtzeit

![Beispiel](notebook/videos/cars_on_the_road.mp4)

#### Erkennung von "Fabian" (Nachbar's Katze) in Echtzeit

![Beispiel](notebook/videos/cars_on_the_road.mp4)

## Training

