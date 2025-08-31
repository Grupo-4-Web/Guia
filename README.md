# Guia para contribuir

Este guia fornece instruções sobre como contribuir para o projeto. O GitHub também possui um [Guia para iniciantes](https://docs.github.com/pt/get-started/quickstart) que pode ser útil.

## Informações básicas

Esta organização possui vários repositórios. Cada repositório possui um propósito específico, além de um arquivo `README.md` que explica como executar o projeto.

## Como contribuir

> [!NOTE]
> O guia abaixo utiliza o Git para clonar o repositório e fazer commits. Se você sentir mais confortável usando uma interface gráfica, sinta-se à vontade para usar ferramentas como [GitHub Desktop](https://desktop.github.com/download/), mas saiba que o guia a seguir é baseado no uso do terminal.

> [!NOTE]
> Certifique-se de ter o Git instalado em sua máquina. Você pode baixar e instalar o Git a partir de [git-scm.com](https://git-scm.com/).

1. **Clonar o repositório**: Use o comando `git clone <URL do repositório>` para clonar o repositório localmente.

   Exemplo:

   ```bash
   git clone https://github.com/Grupo-4-Web/Guia.git
   ```

2. **Abrir o projeto**: Navegue até o diretório do projeto clonado e abra-o em sua IDE favorita (como VSCode, IntelliJ, etc.).

3. **Instalar dependências**: Siga as instruções no arquivo `README.md` do repositório para instalar todas as dependências necessárias.

4. **Configurar variáveis de ambiente**: Se o projeto requer variáveis de ambiente, crie um arquivo `.env` na raiz do projeto e adicione as variáveis necessárias conforme especificado no `README.md`. Essas variáveis não devem ser compartilhadas publicamente.

5. **Faça sua branch**: Crie uma nova branch para suas alterações usando o comando:

   ```bash
   git checkout -b <seu-nome>/<descrição-da-alteração>
   ```

   Essa nova branch cria uma nova linha do tempo para suas alterações, permitindo que você trabalhe sem afetar a branch principal.

   Exemplo:

   ```bash
   git checkout -b italo/corrigir-bug-login
   ```

6. **Faça suas alterações**: Realize as alterações necessárias no código. Certifique-se de seguir as boas práticas de codificação e os padrões do projeto.

7. **Commit suas alterações**: Depois de fazer as alterações, use o comando `git add .` para adicionar todas as alterações ao estágio de commit. Em seguida, faça o commit com uma mensagem descritiva:

   ```bash
   git commit -m "Descrição clara e concisa das alterações feitas"
   ```

8. **Push suas alterações**: Envie suas alterações para o repositório remoto usando o comando:

   ```bash
   git push origin <sua-branch>
   ```

   Os passos 7 e 8 podem ser repetidos várias vezes enquanto você trabalha em suas alterações, fazendo commits frequentes para salvar seu progresso.

9. **Criar um Pull Request (PR)**: Vá até o repositório no GitHub e crie um Pull Request da sua branch para a branch principal (`main`). Descreva claramente as alterações que você fez e por que elas são necessárias. Para mais detalhes, consulte [Como criar uma solicitação de pull](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).

10. **Revisão de código**: Outros membros da equipe revisarão seu Pull Request. Eles podem sugerir mudanças ou aprovar suas alterações. Esteja aberto a feedback e faça as alterações necessárias.

11. **Mesclar o Pull Request**: Depois que seu Pull Request for aprovado, o mantenedor do repositório pode mesclá-lo na branch principal usando o botão "Merge pull request" no GitHub.

12. **Atualizar sua branch local**: Após a mesclagem, certifique-se de atualizar sua branch local com as últimas alterações da branch principal:
    ```bash
    git checkout main # para voltar para a branch principal
    git pull origin main # para obter as últimas alterações
    ```

## Boas práticas

- **Commits frequentes**: Faça commits frequentes com mensagens claras para facilitar o rastreamento das alterações.
- **Revisão de código**: Sempre revise o código antes de fazer um commit para garantir que ele esteja limpo e funcional.
- **Documentação**: Atualize a documentação conforme necessário para refletir suas alterações.
- **Comunicação**: Mantenha uma comunicação aberta com a equipe para garantir que todos estejam alinhados.

## Recursos adicionais

- [Guia do GitHub para iniciantes](https://docs.github.com/pt/get-started/quickstart)
- [Documentação oficial do Git](https://git-scm.com/doc)
- [Boas práticas de Git](https://chris.beams.io/posts/git-commit/)
