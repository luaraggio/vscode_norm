Como automatizar norminette no vs code?
  - Sempre que salvar um arquivo, a norma será formatada automaticamente.

1. Clonar repositório do c_formatter_42 e guardar o path do lugar onde clonou para, posteriormente, adicionar às configurações do vs code.
git@github.com:luaraggio/c_formatter_42.git

2. pip3 install c_formatter_42

3. Baixar extensão no vs code
https://marketplace.visualstudio.com/items?itemName=keyhr.42-c-format

4. Abrir settings.json no vs code e adicionar os seguintes elementos:
[],

  "editor.defaultFormatter": "keyhr.42-c-format",
  "[c]": {
    "editor.defaultFormatter": "keyhr.42-c-format"
  },
  "42-c-format.path": "path_do_repositorio_que_foi_clonado/c-formatter-42",
  "editor.formatOnSave": true
}
