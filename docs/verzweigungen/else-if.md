# Verzweigung

Es gibt außerdem die Möglichkeit mehrere If- und Else-Anweisungen zu kombinieren. Dies ist mit der Else-If-Anweisung möglich.\
Schlägt dabei eine If-Prüfung fehl, wird die Prüfung der nächsten Else-If-Anweisung durchgeführt.

### Beispiel
Zum vorherigen Beispiel ist zusätzlich zu prüfen, ob die Person ein Kind ist.

```cs
int alter = 10;

if (alter < 12)
{
    Console.WriteLine("Die Person ist ein Kind!");
}
else if (alter < 18)
{
    Console.WriteLine("Die Person ist ein Teenager!");
}
else
{
    Console.WriteLine("Die Person ist volljährig");
}
```
??? quote "Ausgabe"
    ``` text
    Die Person ist ein Kind!
    ```

!!! info "Erklärung"
        Da die Prüfung in Zeile 3 fehlschlägt, wird die Nächste Prüfung in Zeile 7 ausgeführt. Da diese Prüfungen erfolgreich ist, erscheint die entsprechende Ausgabe.

!!! info

	1. Das [`using`-Keyword](#using) stellt sicher, dass der StreamReader wieder geschlossen wird
	1. Hier wird line mit der ersten Zeile von TestDatei.txt initialisiert
	1. Das "Verarbeiten" ist hier eine einfach Konsolenausgabe. Natürlich kann hier alles erdenkliche mit der Zeile passieren.
	1. Hier wird die nächste Zeile eingelesen. Dieser Schritt ist in der Regel immer der letzte Schritt in der Schleife, da danach wieder geprüft werden muss, ob es noch etwas einzulesen gibt.
