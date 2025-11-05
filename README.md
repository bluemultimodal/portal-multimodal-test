# Blue Multimodal - Portal de Testes

Este repositório contém os arquivos de um aplicativo de planejamento multimodal para fins de teste e demonstração. O aplicativo foi ajustado para ser publicado online gratuitamente usando o GitHub Pages.

## O que foi corrigido?

O aplicativo não estava funcionando no GitHub Pages porque o código-fonte (em formato `.tsx`) não estava sendo "traduzido" para JavaScript, que é a linguagem que os navegadores entendem. Adicionamos uma ferramenta (Babel) que faz essa tradução em tempo real, diretamente no navegador. Agora, a publicação deve funcionar sem problemas.

## Como Publicar e Testar na Internet (Passo a Passo)

Siga estes passos para ter seu próprio link de teste do aplicativo. Se você já tem um repositório, pode pular o Passo 1 e apenas enviar os arquivos atualizados (Passo 2).

### Passo 1: Crie um Repositório no GitHub

1.  Acesse o [GitHub](https://github.com/) e faça login.
2.  Crie um **novo repositório**. Você pode chamá-lo de `portal-multimodal-test`, por exemplo.
3.  Marque-o como **Público** para que o GitHub Pages funcione.
4.  **Não** inicialize com um README, .gitignore ou licença.

### Passo 2: Envie os Arquivos do Projeto

1.  No seu novo repositório, clique em **"uploading an existing file"**.
2.  **Arraste e solte todos os arquivos** do projeto (incluindo `index.html`, `App.tsx`, a pasta `components`, etc.) para a área de upload. Se você já tinha os arquivos lá, envie os novos para substituí-los.
3.  Após o upload, clique em **"Commit changes"**.

### Passo 3: Ative o GitHub Pages (A Etapa Mais Importante)

1.  No seu repositório, vá para a aba **"Settings"** (Configurações).
2.  No menu lateral esquerdo, clique em **"Pages"**.
3.  Na seção "Build and deployment", em "Source", selecione **"Deploy from a branch"**.
4.  Logo abaixo, na seção **"Branch"**, configure o seguinte:
    -   **Branch:** Selecione a branch `main` (ou `master`).
    -   **Folder:** Selecione a opção **`/ (root)`**. *Esta é a opção correta. Não selecione `/docs`.*
5.  Clique em **"Save"**.

### Passo 4: Acesse seu Aplicativo

- Após salvar, o GitHub começará a publicar seu site. Pode levar 1 ou 2 minutos.
- A página de configurações do GitHub Pages mostrará uma mensagem e, quando estiver pronto, exibirá um banner verde com o link para o seu aplicativo.
- O link terá o formato: `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`
- **Pronto!** Agora você pode acessar esse link de qualquer dispositivo.

## Funcionalidades para Teste

### Armazenamento de Dados no Dispositivo (Offline)

O aplicativo **salva todos os seus dados diretamente no navegador do seu dispositivo** (celular, tablet ou computador) usando `localStorage`. Ao fechar e reabrir o site, seus dados estarão lá.

### Backup e Restauração Local

Na tela de **Configurações**, você pode:

- **Criar Backup:** Gera um arquivo `.json` com todos os dados atuais e o salva no seu dispositivo.
- **Restaurar:** Carrega um arquivo de backup `.json`, substituindo os dados atuais pelos do arquivo.
