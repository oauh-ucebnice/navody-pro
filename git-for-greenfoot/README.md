# Použití Gitu a GitHubu s Greenfootem

## Co používáme
1. _Git_ - nástroj pro sledování historie projektu
2. _GitHub_ a podobné služby - servery pro sdílení kódu
3. _GitHub Desktop_ ... aplikace - grafické uživatelské rozhraní ke Gitu, propojené s GitHubem


## Vytvoření účtu na GitHubu (pokud již nemáte)

Pro vytvoření účtu použijte [návod na OAUH učebnice](https://github.com/oauh-ucebnice/github-registrace).

## Instalace GitHub Desktop

<details><summary>Postup...</summary>

1. <br />![](img/git-gft_010_ghdesk-install_0010_download.png)
1. <br />![](img/git-gft_010_ghdesk-install_0020_login.png)
1. <br />![](img/git-gft_010_ghdesk-install_0030_finished.png)

</details>


## Založení repozitáře a vytvoření projektu Greenfootu

### Založení repozitáře

> Repozitář vytvoří pouze jeden člen skupiny. Tento člen publikuje repozitář na GitHub. Ostatní členové skupiny si pak repozitář naklonují.

<details><summary>Postup...</summary>

1. <br />![](img/git-gft_020_create-repo_0010_create.png)
1. <br />![](img/git-gft_020_create-repo_0020_repo-name.png)
1. <br />![](img/git-gft_020_create-repo_0030_publish.png)
1. <br />![](img/git-gft_020_create-repo_0040_private.png)
1. <br />![](img/git-gft_020_create-repo_0050_pruzkumnik-repo.png)
1. <br />![](img/git-gft_020_create-repo_0060_web-repo.png)
</details>

### Kontrola a povolení přístupu ostatním

Repozitář nastavujeme jako veřejný, takže jeho obsah může vidět kdokoli. Ale přispívat do něj může ve výchozím nastavení jen autor. Ostatním členům skupiny musí autor repozitář zpřístupnit.

<details><summary>Postup...</summary>

1. <br />![](img/git-gft_030_share_0010_settings.png)
1. <br />![](img/git-gft_030_share_0020_collaborators.png)

Uvedeným členům skupiny pošlete pozvánku pomocí _Add Member_. Pozvánka jim dojde mailem a zároveň se zobrazí na GitHubu. Teprve až pozvánku přijmou, můžou do repozitáře přispívat.

> Pokud byste omylem vytvořili privátní rezpozitář (není viditelný veřejně), můžete toto nastavení změnit viz žlutá šipka.

</details>


## Zápis kódu a odeslání změn na GitHub

<details><summary>Postup...</summary>

1. Při první vytvoření do repozitáře zkopírujeme kód<br />![](img/git-gft_040_code_0010_copy.png)

> Později už měníme existující kód. Otevřeme si projekt v&nbsp;Greenfootu a píšeme stejně, jak jsme zvyklí.

2. Každou novou funkčnost bychom měli zapsat jako nový commit<br />
![](img/git-gft_040_code_0020_commit.png)
3. Uložené commity poté můžeme odeslat do vzdáleného repozitáře<br />![](img/git-gft_040_code_0030_push.png)
4. Po odeslání commitů se aktuální stav projektu objeví i ve vzdáleném repozitáři<br />![Aktualizovaný repozitář na webu](img/git-gft_040_code_0050_web-repo.png)

> Dokud neprovedeme operaci „push“, ostatní členové projektu naše změny neuvidí.

Než si projekt otevřeme po delší době, měli bychom si načíst změny, které provedli mezitím naši kolegové:

1. <br />![](img/git-gft_040_code_0040_fetch.png)


</details>


## Stažení existujícího projektu z GitHubu

<details><summary>Postup...</summary>

1. <br />![](img/git-gft_050_clone_0010_url.png)
1. <br />![](img/git-gft_050_clone_0020_clone.png)
1. <br />![](img/git-gft_050_clone_0030_enter-url.png)

</details>


## Stažení nových změn ze vzdáleného rezpozitáře

<details><summary>Popis a postup...</summary>

V&nbsp;době, kdy s&nbsp;repozitářem nepracujete, mohlo dojít k&nbsp;nahrání nových commitů do vzdáleného repozitáře.
Mohlo to nastat tak, že:
- Někdo z&nbsp;vašich kolegů nahrál do vzdáleného repozitáře své úpravy.
- Vy jste provedli úpravy projektu na jiném počítači a nahráli změny do repozitáře.

Před začátkem další práce je třeba tyto commity stáhnout tak, abyste měli k&nbsp;dispozici aktuální verzi kódu (pozor, toto se neprovádí automaticky).

1. <br />![](img/git-gft_040_code_0040_fetch.png)

</details>
