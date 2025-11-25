# Instalace Flutteru ve Windows

## Instalace Flutter SDK

1. <br />![](img/install-vscode/flutter_install-vscode_0010_plugin.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0020_plugin-wait.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0030_plugin-done.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0050_download-sdk.png)
1. Jako cestu pro instalaci SDK **vytvořte novou složku `develop`** ve své domovské složce.  
Například: `C:\Users\dvorak_adam\develop`
1. Čekej na dokončení instalace...<br />![Čekej...](img/install-vscode/flutter_install-vscode_0060_downloading.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0070_add-to-path.png)
1. Vyber druh aplikace *Application*:  
   ![Vyber *Application*](img/install-vscode/flutter_install-vscode_0080_new-app-project.png)
1. Na projekty si **vytvoř novou složku Flutter** ve své domovské složce.  
   Například: `C:\Users\dvorak_adam\Flutter`
1. <br />![](img/install-vscode/flutter_install-vscode_0100_trust-authors.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0120_debug-app.png)

## Flutter Doctor

Po instalaci je dobré zkontrolovat stav instalace pomocí příkazu:
```shell
flutter doctor
```
1. <br />![](img/install-vscode/flutter_install-vscode_0200_vscode.png)

Zatím nám chybí doinstalovat:
1. SDK pro aplikace Windows a Visual Studio (ne jen Visual Studio Code – to nestačí)
2. Android Studio a SDK pro tvorbu aplikací pro Android.

Potřebujeme alespoň jednu z těchto součástí, abychom mohli začít překládat první aplikace Flutterem.

> Pokud už máš něco z toho nainstalované z dřívějška, můžeš odpovídající krok přeskočit.

## Instalace Windows SDK
1. Odkaz pro instalaci ti zobrazí Flutter Doctor. Zavede tě na stránky Visual Studia:  
   ![](img/install-vscode/flutter_install-vscode_0210_vscode-web.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0220_run-installer.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0230_vs-installer.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0240_downloading.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0250_select-desktop-cpp.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0260_installing.png)
1. <br />![](img/install-vscode/flutter_install-vscode_0270_ready.png)

Nyní již můžeš spustit svoji první aplikaci:  
![](img/install-vscode/flutter_install-vscode_0280_running.png)