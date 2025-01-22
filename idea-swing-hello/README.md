# Hello World s GUI v Javě (IDEA + SWING)

Předpokládáme, že vývojové prostředí IntelliJ IDEA máš již nainstalované.

> Návod je vytvořen ve verzi 2024.3.1.1.

## Instalace pluginu Swing GUI Designer

Nástroje pro tvorbu grafického rozhraní jsou součástí pluginu Swing GUI Designer. Ten stačí nainstalovat jednou. U dalších projektů už tento krok nebude třeba:

![](img/swing-idea_0010_plugins.png)
![](img/swing-idea_0020_install-plugin.png)

## Vytvoření projektu Hello GUI

Nyní již vytvoříš projekt stejně jako normálně.

![](img/swing-idea_0030_project.png)
![](img/swing-idea_0040_name.png)

Do projektu je třeba přidat formulář okna.

![](img/swing-idea_0050_gui-form.png)
![](img/swing-idea_0060_form-name.png)
![](img/swing-idea_0070_git.png)

Do formuláře nyní můžeš přetáhnout grafické prvky. Zkus třeba tlačítko.

![](img/swing-idea_0080_button.png)

Prvky je vhodné pojmenovat. Nenechávej prvkům výchozí pojmenování `button1` apod.

![](img/swing-idea_0090_bt-descript.png)

Pojmenovat je třeba i hlavní panel formuláře. Pomocí tohoto názvu pak panel propojíš s&nbsp;oknem.

![](img/swing-idea_0100_pn-descript.png)

Nyní zapiš kód hlavního okna:
1. Nezapomeň na `extends JFrame`, aby se aplikace uměla chovat jako okno (využíváme dědičnost ze třídy `JFrame`).
2. Vytvoř si pomocnou metodu `initComponents`, kterou zavoláš v&nbsp;konstruktoru
3. Potřebujeme:
    - Přiřadit k&nbsp;oknu vytvořený panel s&nbsp;formulářem: `setContentPane` &mdash; zde použij název hlavního panelu vytvořeného formuláře
    - Nastavit titulek okna: `setTitle` &mdash; text se objeví v titulkové liště okna (nahoře)
    - Zajistit, aby se okno při stisknutí zavíracího tlačítka zavřelo: `setDefaultCloseOperation(EXIT_ON_CLOSE)`
    - Nastavit velikost okna: `pack()` nebo `setSize(x, y)`

Celý kód máš zde:
```java
import javax.swing.*;

public class HelloFrame extends JFrame {
    private JButton btStart;
    private JPanel pnMain;

    public HelloFrame() {
        initComponents();
    }

    private void initComponents() {
        setContentPane(pnMain);
        setTitle("Hello GUI");
        setDefaultCloseOperation(EXIT_ON_CLOSE);
        pack();
        //setSize(300, 300);
       btStart.addActionListener(e -> pozdrav());
   }
}
```

![](img/swing-idea_0110_frame-code.png)

V&nbsp;metodě `main` pak stačí vytvořit objekt okna a nastavit, aby bylo viditelné:
```java
public class Main {
    public static void main(String[] args) {
        HelloFrame frame = new HelloFrame();
        frame.setVisible(true);
    }
}
```
![](img/swing-idea_0120_main-code.png)

## Reakce na tlačítko

Aby tlačítko něco dělalo, musíš mu přiřadit _listener_. Přiřaď mu metodu, která se spustí při stisknutí tlačítka:
```java
import javax.swing.*;

public class HelloFrame extends JFrame {
    private JButton btStart;
    private JPanel pnMain;

    public HelloFrame() {
        initComponents();
    }

    private void initComponents() {
        setContentPane(pnMain);
        setTitle("Hello GUI");
        setDefaultCloseOperation(EXIT_ON_CLOSE);
        pack();
        //setSize(300, 300);
        btStart.addActionListener(e -> pozdrav());
    }

    private void pozdrav() {
        JOptionPane.showMessageDialog(
                this, "Hello GUI!");
    }
}
```
![](img/swing-idea_0130_listener.png)

Nyní můžeš kód spustit:
![](img/swing-idea_0140_run.png)
![](img/swing-idea_0150_result.png)

Pro lepší manipulaci s&nbsp;oknem můžeš oknu nastavit přesné rozměry, aby okno bylo větší:
![](img/swing-idea_0160_size.png)