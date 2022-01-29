# Como fazer um _pull request_ corretamente

- Criar um _fork_ pessoal do projeto no GitHub;
- Clonar o _fork_ em sua máquina local. Seu repositório remoto do GitHub é conhecido por `origin`;
- Adicionar o repositório original como um remoto chamado `upstream`;
- Se você criou o _fork_ há algum tempo, certifique-se de realizar pull das alterações no seu repositório local;
- Criar um nova _branch_ para trabalhar nela! Ramifique da `develop`, se existir; caso contrário, crie da `main`;
- Implementar/corrigir sua _feature_, não esquecendo de comentar o seu código;
- Siga o estilo de código do projeto em questão, inclusive a indentação;
- Se o projeto apresentar testes, execute-os;
- Escreva ou adapte os testes, conforme necessário;
- Adicionar ou alterar a documentação, conforme necessário;
- Junte seus _commits_ em um único _commit_ com o [rebase interativo][A] do Git. Criar uma nova _branch_, caso seja necessário;
- _Push_ sua _branch_ para seu _fork_ do GitHub, o remoto `origin`;
- Do seu _fork_, abra uma _pull request_ na _branch_ correta. Aponte a _branch_ `develop` do projeto se existir; caso contrário, vá para `main`;
- Uma vez que o _pull request_ for aprovado e mesclado, é possível extrair as alterações do `upstream` para seu repositório local e excluir suas _branchs_ extras;
- Pronto! Muito obrigado pela contribuição.

> Sempre escreva suas mensagens de commit no tempo presente. Sua mensagem de commit deve descrever o que o commit, quando aplicado, faz com o código – não o que você fez com o código.

<!-- MARKDOWN LINKS>
<!-- SITES -->
[A]: https://www.atlassian.com/br/git/tutorials/rewriting-history/git-rebase









Contributing
----------------------------------

1. File an issue to notify the maintainers about what you're working on.
2. Fork the repo, develop and test your code changes, add docs.
3. Make sure that your commit messages clearly describe the changes.
4. Send a pull request.

File an Issue
----------------------------------

Use the issue tracker to start the discussion. It is possible that someone
else is already working on your idea, your approach is not quite right, or that
the functionality exists already. The ticket you file in the issue tracker will
be used to hash that all out.

Style Guides
-------------------
1. Write in UTF-8 in Python 3
2. User modular architecture to group similar functions, classes, etc. 
3. Always use 4 spaces for indentation (don't use tabs)
4. Try to limit line length to 80 characters
5. Class names should always be capitalized
6. Function names should always be lowercase
7. Look at the existing style and adhere accordingly

Fork the Repository
-------------------

Be sure to add the relevant tests before making the pull request. Docs will be
updated automatically when we merge to `master`, but you should also build
the docs yourself and make sure they're readable.

Make the Pull Request
---------------------

Once you have made all your changes, tests, and updated the documentation,
make a pull request to move everything back into the main branch of the
`repository`. Be sure to reference the original issue in the pull request.
Expect some back-and-forth with regards to style and compliance of these
rules.
