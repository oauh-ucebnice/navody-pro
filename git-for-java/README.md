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
    git config --global user.email="vas-email@domena.cz"
    git config --global user.name="Uživatelské jméno na GitHubu"
    ```
    <br />![](img/github-key_015_git-config.png)
1. Spusťte `ssh-keygen` a nechte si vygenerovat klíče:
    ```bash
    ssh-keyget -t rsa
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
1. <br />![](img/github-ij_500_copy-ssh-link.png)

</details>

## Stažení existujícího projektu z GitHubu do IntelliJ

<details><summary>Postup...</summary>

1. <br />![](img/github-ij_510_get-from-vcs.png)
1. <br />![](img/github-ij_520_clone.png)

</details>