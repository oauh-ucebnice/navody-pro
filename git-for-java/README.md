# Použití Gitu a GitHubu s IntelliJ IDEA

## Vytvoření účtu na GitHubu (pokud již nemáte)

Pro vytvoření účtu použijte [návod na OAUH učebnice](https://github.com/oauh-ucebnice/github-registrace).


## Instalace Gitu (pokud již nemáte)

Ve škole tento krok není třeba, protože je Git již nainstalován.

   <details><summary>Postup...</summary>
1. Git stáhnete ze stránek: [git-scm.com](https://git-scm.com/download/).

1. Při instalaci je třeba potvrdit větší množství voleb, ale většinu z&nbsp;nich lze ponechat ve výchozím nastavení. Změňte si pouze výchozí editor pro úpravu commit message.

   <details><summary>První část postupu (zvolte sami či ponechte výchozí)...</summary>

    1. <br />![](img/git-install_010_download.png)
    1. <br />![](img/git-install_020_64bit.png)
    1. <br />![](img/git-install_030_licence.png)
    1. <br />![](img/git-install_040_folder.png)
    1. <br />![](img/git-install_050_components.png)
    1. <br />![](img/git-install_060_menu.png)

   </details>


1. Zvolte textový editor pro instalaci<br />
   - Zvolte si editor podle své volby. Můžete například použít výchozí editor pro Windows: Notepad
   > Pokud jste na editor _vim_ zvyklí, samozřejmě si můžete ponechat _vim_. Pro běžného uživatele počítače bez dalších zkušeností ale _vim_ není příliš intuitivní na ovládání!

   - ![](img/git-install_070_no-vim.png)<br />![](img/git-install_075_use-notepad.png).

1. Zbytek instalace už nejspíš můžete ponechat beze změny (volby se mohou lišit)

   <details><summary>Druhá část postupu (zvolte sami či ponechte výchozí)...</summary>

    1. <br />![](img/git-install_080_main-branch.png)
    1. <br />![](img/git-install_090_both-git-bash.png)
    1. <br />![](img/git-install_100_bundled-ssh.png)
    1. <br />![](img/git-install_110_openssh.png)
    1. <br />![](img/git-install_120_crlf.png)
    1. <br />![](img/git-install_130_tty.png)
    1. <br />![](img/git-install_140_fast-forward.png)
    1. <br />![](img/git-install_150_credential-manager.png)
    1. <br />![](img/git-install_160_extra.png)
    1. <br />![](img/git-install_170_experimental.png)
    1. <br />![](img/git-install_180_install.png)


   </details>

</details>


## Vložení klíče na GitHub

<details><summary>Postup...</summary>

1. <br />![](img/github-key_010_cmd.png)
1. Nastavte si uživatelské jméno pro zápis autora změn.<br />Použijte uživatelské jméno a e-mail vašeho účtu na GitHubu:
    ```bash
    git config --global user.email "vas-email@domena.cz"
    git config --global user.name "Uživatelské jméno na GitHubu"
    ```
    <br />![](img/github-key_015_git-config.png)
1. Spusťte `ssh-keygen` a nechte si vygenerovat klíče:
    ```bash
    ssh-keygen -t rsa
    ```
    <br />![](img/github-key_020_ssh-keygen.png)
    1. Pokud už jste někdy klíč vytvářeli, můžete použít ten původní.
    1. Cestu ke klíči ponechte výchozí.
    1. Heslo doporučujeme nezadávat, protože byste ho museli zadávat při každém commitu.
1. <br />![](img/github-key_030_ssh-dir.png)
1. <br />![](img/github-key_040_ssh-content.png)
1. <br />![](img/github-key_050_idrsapub-open.png)
1. <br />![](img/github-key_060_notepad.png)
1. <br />![](img/github-key_070_notepad-content.png)
1. <br />![](img/github-key_080_add-key.png)
1. <br />![](img/github-key_090_new-key.png)
1. <br />![](img/github-key_100_add-key.png)

</details>

## Vytvoření projektu IntelliJ a odeslání na GitHub
<details><summary>Postup...</summary>

1. <br />![](img/github-ij_010_new-project.png)
1. <br />![](img/github-ij_020_create-git-repo.png)
1. <br />![](img/github-ij_030_share-github.png)
1. <br />![](img/github-ij_045_repo-account-set.png)
1. <br />![](img/github-ij_050_no-settings.png)
1. <br />![](img/github-ij_060_gitignore.png)
1. <br />![](img/github-ij_065_gitignore-input.png)

</details>

## Odeslání změn na GitHub

<details><summary>Postup...</summary>

1. <br />![](img/github-ij_070_commit.png)
1. <br />![](img/github-ij_080_history.png)
1. <br />![](img/github-ij_090_push.png)
1. <br />![](img/github-ij_095_push-list.png)
1. <br />![](img/github-ij_100_repo.png)
1. <br />![](img/github-ij_110_repo-content.png)

</details>

## Stažení existujícího projektu z GitHubu do IntelliJ

<details><summary>Postup...</summary>

1. Zkopírujte si adresu repozitáře:<br />![](img/github-ij_500_copy-ssh-link.png)
1. Zadejte adresu do úvodního okna po spuštění IntelliJ:<br />
   Pokud máte otevřen jiný projekt, zavřete ho.<br />![](img/github-ij_510_get-from-vcs.png)
1. <br />![](img/github-ij_520_clone.png)

</details>

## Stažení nových commitů ze vzdáleného rezpozitáře

<details><summary>Postup...</summary>

V&nbsp;době, kdy s&nbsp;repozitářem nepracujete, mohlo dojít k&nbsp;nahrání nových commitů do vzdáleného repozitáře.
Mohlo to nastat tak, že:
- Někdo z&nbsp;vašich kolegů nahrál do vzdáleného repozitáře své úpravy.
- Vy jste provedli úpravy projektu na jiném počítači a nahráli změny do repozitáře.

Před začátkem další práce je třeba tyto commity stáhnout tak, abyste měli k&nbsp;dispozici aktuální verzi kódu (pozor, toto se neprovádí automaticky).

1. Otevřete si projekt v&nbsp;IntelliJ a stiskněte „modrou šipku dolů“ („Update project“):<br />
   ![Klikněte na modrou šipku „Update project...“](img/github-ij_600_pull.png)
1. Pokud jste provedli nové commity a ve vzdáleném repozitáři vznikly také nové commity, můžete je zařadit do historie dvojím způsobem:
   1. _merge_ &hellip; commity budou řazeny časově, můžou být tedy promíchány commity z&nbsp;lokálního repozitáře a mezi nimi commity ze vzdáleného. (Hodí se, pokud jste prováděli navzájem nezávislé commity a chcete v&nbsp;historii zachovat časovou posloupnost akcí.)
   2. _rebase_ &hellip; v&nbsp;historii budou nejprve všechny commity ze vzdáleného repozitáře a pak teprve všechny nové commity z&nbsp;lokálního repozitáře. (Hodí se, pokud jste dělali lokální více commitů, které ale dohromady tvoří jednu akci.)
   
   ![Vyberte strategii řazení nových commitů „merge“ nebo „rebase“...](img/github-ij_610_merge-rebase.png)
1. Pokud některé vzdálené commity upravují stejné řádky, které jste mezitím měnil(a) i vy, dojde ke _kolizi_ a IntelliJ zobrazí vedle sebe kód ze vzdáleného repozitáře a z&nbsp;vašeho lokálního repozitáře. Musíte pak rozhodnout, jak má výsledek vypadat.
1. Nyní budete mít v&nbsp;historii všechny commity z&nbsp;lokálního i vzdáleného repozitáře a aktuální kód.

</details>
