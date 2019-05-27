## E-Commerce

Auch für E-Commerce gibt es eine Anzahl Plugins. Die meisten bauen auf einem "Freemium"-Geschäftsmodell auf, das bedeutet, die Basisversion des Plugins gibt es kostenlos, Zusatzfunktionen müssen gegen Bezahlung erworben werden.
Zu den wichtigsten Zusatzfunktionen gehört die Anbindung an Payment Service Provider. Wenn man bei einem Onlineshop Bezahlung via Kreditkarte akzeptieren will, benötigt man aber nicht nur das entsprechende Plugin, sondern muss mit einem Payment Service Provider (PSP) einen Vertrag haben. Je nachdem mit welchem PSP man zusammenarbeiten will, ändert sich unter Umständen auch die Auswahl an Shopsystemen für welches ein fertiges Plugin besteht. Natürlich liesse sich ein passendes Plugin auch selber entwickeln. Dies ist aber in den meisten Fällen ein Aufwand den man sich mit dem Erwerb eines kostenpflichtigen Plugins besser ersparen sollte. Eine gute Übersicht über verschiedene Lösungen bietet die Firma [customweb.ch](http://www.customweb.com/de) an, die sich auf die Software-Entwicklung im Bereich des Electronic Payment spezialisisert hat. Unter dem Namen [sellXed](http://www.sellxed.com/de) bietet dieser Schweizer Anbieter Plugins für alle gängigen WordPress Shopsysteme (und viele andere) in Zusammenhang mit den meisten relevanten Payment Service Providern [^psp] an.

Eine gute Übersicht über in der Schweiz verbreitete Payment Service Provider gibt es bei openstream.ch: [Zahlungsarten für den Schweizer Onlineshop](https://www.openstream.ch/blog/zahlungsarten-schweiz/).

Das mit Abstand meistverbreitete WordPress Shop-Plugin ist [woocommerce](https://wordpress.org/plugins/woocommerce/). Dieses Plugin entstand aus einem Fork von [Jigoshop](https://www.jigoshop.com/) durch den Themenanbieter [WooThemes](https://www.woothemes.com/), der einen Teil der ursprünglichen Entwickler abwarb. Im Mai 2015 wurde WooCommerce von Automattic  [akquiriert](http://ma.tt/2015/05/woomattic/).

Um ausschliesslich digitale Produkte zu verkaufen ist [Easy Digital Downloads (EDD)](https://easydigitaldownloads.com/) weit verbreitet. ([WordPress.org](https://wordpress.org/plugins/easy-digital-downloads/))

### Wie eine Online Zahlung in etwa abläuft und welche Parteien dabei involviert sind

Die folgenden Grafiken von der [sellXed Webseite](http://www.sellxed.com/de/funktionsweise) zeigen die Funktionsweise des Zahlunsablaufs auf einer Webseite und die beteiligten Akteure.

![Funktionsweise des sellXed Plugins](images/v4.5/Custoweb_Process_cw_4.png)

![Funktionsweise des sellXed Plugins](images/v4.5/payment_process_1.png)

1. Der Kunde sucht sich ein Produkt im Online Shop aus und drückt auf "Kaufen".
2. Der Kunde wählt eine Zahlungsoption und gibt die entsprechenden Zahlungsinformationen ein. Die Zahlungs Module von sellXed verschlüsseln die Nachricht mit einem Stempel und übermitteln diese über eine gesicherte Verbindung an den PSP.
3. Der PSP leitet diese Daten wiederum an den Acquirer weiter.
4. Der Acquirer schickt die Zahlungsinformationen an die Bank des Kunden - ebenfalls über einen gesicherten Kanal.
5. Basierend auf der Kreditlimite des Kunden wird die Transaktion von der Issuing Bank entweder akzeptiert oder abgelehnt. Die Bestätigungs- / Ablehnungsnachricht wird wiederum zurück zum PSP geschickt.
6. Der Acquirer löst nun die Belastung beim Issuer aus und veranlasst eine Überweisung an die Hausbank des Händlers welche er/sie im Kreditkartenakzeptanzvertrag hinterlegt hat.
7. Der PSP übermittelt die digitale Quittung an die Shop-Seite sowie an den Kunden, worauf die Quittung dann vom sellXed Zahlungs Modul geprüft wird. Nur wenn die Sicherheitsmerkmale der ursprünglich abgeschickten Nachricht entsprechen und der PSP die erfolgreiche Bezahlung bestätigt, wird im Shop eine Bestellung angelegt. Im Falle von Betrug oder sonstigen Problemen werden die Bestellungen im Shop durch das Zahlungs Modul entsprechend markiert.
8. Die Ware kann nun versendet werden.

[^psp]: Payment Service Provider, Anbieter, welcher die Anbindung an Bezahllösungen anbietet.