# Discountagreement Exchange Format
Das im Folgenden definierte Schema für XML-Dateien dient dem strukturierten Austausch (Import/Export in [DataHive](http://www.scireum.de/datahive/vorteile)) von Konditionsvereinbarungen (Discountagreements).

# Aufbau
XML Dateien, welche diesem Schema entsprechen, sind in zwei Hauptteile unterteilt: Voraussetzungen (Prerequisites), in denen Typen definiert und Beschreibungen festgelegt werden auf welche später Bezug genommen werden kann, sowie ein Teil zur eigentlichen Konditionsvereinbarung (DiscountAgreement).
## Voraussetzungen (Prerequisites)
In diesem XML-Abschnitt werden zum einen Roundingdescriptions (optional), als auch alle Discounttypes aufgeführt. Diese werden eindeutig über eine UUID festgelegt und können später innerhalb von Discountgroups über diese referenziert werden.
## Konditionsvereinbarung (DiscountAgreement)
Dieser XML-Abschnitt beschreibt die eigentliche Konditionsvereinbarung und deren festgelegte Werte. Hier werden insbesondere alle Discountgroups aufgeführt, welche Bezug auf die Discounttypes nehmen, die innerhalb der Prerequisites aufgelistet wurden.