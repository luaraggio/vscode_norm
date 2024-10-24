<h1 align="center">Como automatizar norminette no VS Code? 👾</h1>
<p align="">
  Ao salvar um arquivo no VS Code, será possível formatar automaticamente o código para que se enquadre na norminette.
</p>

<hr>

<h2>Passo a Passo</h2>

<h3>1. Clonar o Repositório do c_formatter_42</h3>
<p>Primeiro, clone o repositório oficial do <code>c_formatter_42</code> no local desejado e guarde o caminho (path) do repositório, pois ele será usado mais tarde nas configurações do VS Code.</p>

<pre><code>git clone git@github.com:luaraggio/c_formatter_42.git</code></pre>

<h3>2. Instalar o c_formatter_42 via Pip</h3>
<p>Execute o seguinte comando no terminal para instalar o formatter:</p>

<pre><code>pip3 install c_formatter_42</code></pre>

<h3>3. Baixar a Extensão do 42 Formatter no VS Code</h3>
<p>Baixe a extensão oficial do <code>c_formatter_42</code> diretamente no Marketplace do VS Code. Clique no link abaixo para acessar a extensão:</p>

<a href="https://marketplace.visualstudio.com/items?itemName=keyhr.42-c-format">Baixar Extensão - 42 C Format</a>

<h3>4. Configurar o settings.json no VS Code</h3>
<p>Agora, abra o <code>settings.json</code> do VS Code e adicione as seguintes configurações para que o formatter seja aplicado automaticamente ao salvar arquivos:</p>

<pre><code>
{
  "editor.defaultFormatter": "keyhr.42-c-format",  // Define o 42-formatter como padrão para C
  "[c]": {
    "editor.defaultFormatter": "keyhr.42-c-format"  // Formatar arquivos .c
  },
  "42-c-format.path": "path_do_repositorio_que_foi_clonado/c-formatter-42",  // Caminho para o formatter
  "editor.formatOnSave": true  // Formatar automaticamente ao salvar
}
</code></pre>

<h3>5. Substitua <code>path_do_repositorio_que_foi_clonado</code></h3>
<p>Cuidado para substituir <code>path_do_repositorio_que_foi_clonado</code> pelo caminho correto do diretório onde você clonou o <code>c_formatter_42</code>. Por exemplo, se você clonou o repositório em <code>/Users/teste/c-formatter-42</code>, o campo ficaria assim:</p>

<pre><code>
"42-c-format.path": "/Users/teste/c-formatter-42"
</code></pre>

<h3>6. Teste a Automação</h3>
<p>Agora, abra um arquivo <code>.c</code> no VS Code, faça algumas alterações e veja se ele é automaticamente formatado ao ser salvo. O VS Code aplicará o <code>42-formatter</code> de acordo com a norma.</p>

<hr>

<h2>Contribuição</h2>
<p>Se você encontrar algum problema ou quiser sugerir melhorias, fique à vontade para abrir uma issue ou um pull request no repositório.</p>

<h2>Licença</h2>
<p>Este projeto está licenciado sob a licença MIT. Veja o arquivo <a href="https://github.com/seu-usuario/c-formatter-42/blob/main/LICENSE">LICENSE</a> para mais detalhes.</p>

