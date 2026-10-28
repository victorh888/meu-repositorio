## 🖥️ PASSO A PASSO DO GIT — TERMINAL

Execute os comandos dentro da pasta do repositório. **Atenção: só faça o `git clone` se o aluno ainda não tiver clonado o projeto. Se a pasta do projeto já existir no computador, não repita o clone; apenas entre nela com `cd` e continue.**

>[!IMPORTANT]
> - LIMPAR GIT NA AREA DE TRABALHO
> - ADD GIT IGNORE DA TECNOLOGIA EM QUESTÃO

```shell
git clone https://github.com/nomedeusuariodoaluno/nomedorepositorio.git
cd nomedorepositorio
```

### Configuração da identidade

#### ==🔴GLOBAL (SÓ EM CASA)==

```shell
git config --global user.name "victorh888"
git config --global user.email "vitorhugoribeiroperes@gmail.com"
```

Se outra pessoa usa Git no mesmo computador, use `--local` dentro desta pasta:

#### ==🟢LOCAL (SÓ EM CASA)==
> [!DANGER]
> NO CURSO É PARA USAR ESSE AQUI DE BAIXO! NUNCA, JAMAIS O GLOBAL

```shell
git config --local user.name "victorh888"
git config --local user.email "vitorhugoribeiroperes@gmail.com"
```

### Publicar a alteração do README

Depois de editar ou criar o `README.md` no VS Code, execute:

```shell
git pull
git add .
```

```shell
git commit -m "Mensagem: "
```

```shell
git push
```

Na primeira publicação, configure o remoto uma única vez, somente se este repositório ainda não tiver um remoto configurado:

```shell
git branch -M main
git remote add origin https://github.com/nomedeusuariodoaluno/nomedorepositorio.git
git push -u origin main
```

A configuração `--local` só é necessária se outra pessoa também usa Git no PC; para uso individual, `--global` basta.