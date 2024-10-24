<h1 align="center">Automating Norminette in VS Code 👾</h1>

<p align="">
  When saving a file in VS Code, it is possible to automatically format the code to comply with Norminette.
</p>

<hr>

<h2>Step by Step</h2>

<h3>1. Clone the c_formatter_42 Repository</h3>
<p>First, clone the official <code>c_formatter_42</code> repository to the desired location and keep the repository path (which will be used later in the VS Code settings).</p>

<pre><code>git clone git@github.com:luaraggio/c_formatter_42.git</code></pre>

<h3>2. Install c_formatter_42 via Pip</h3>
<p>Run the following command in the terminal to install the formatter:</p>

<pre><code>pip3 install c_formatter_42</code></pre>

<h3>3. Download the 42 Formatter Extension in VS Code</h3>
<p>Download the official <code>c_formatter_42</code> extension directly from the VS Code Marketplace. Click the link below to access the extension:</p>

<a href="https://marketplace.visualstudio.com/items?itemName=keyhr.42-c-format">Download Extension - 42 C Format</a>

<h3>4. Configure the settings.json in VS Code</h3>
<p>Now, open the <code>settings.json</code> file in VS Code and add the following configuration so that the formatter is automatically applied when saving files:</p>

<pre><code>
{
  "editor.defaultFormatter": "keyhr.42-c-format",  // Set 42-formatter as the default for C
  "[c]": {
    "editor.defaultFormatter": "keyhr.42-c-format"  // Format .c files
  },
  "42-c-format.path": "path_to_the_cloned_repository/c-formatter-42",  // Path to the formatter
  "editor.formatOnSave": true  // Automatically format on save
}
</code></pre>

<h3>5. Replace <code>path_to_the_cloned_repository</code></h3>
<p>Make sure to replace <code>path_to_the_cloned_repository</code> with the correct directory path where you cloned the <code>c_formatter_42</code>. For example, if you cloned the repository to <code>/Users/test/c-formatter-42</code>, the field would look like this:</p>

<pre><code>
"42-c-format.path": "/Users/test/c-formatter-42"
</code></pre>

<h3>6. Test the Automation</h3>
<p>Now, open a <code>.c</code> file in VS Code, make some changes, and see if it is automatically formatted when saved. VS Code will apply the <code>42-formatter</code> according to the Norminette.</p>

<hr>

<h2>Contributing</h2>
<p>If you encounter any issues or want to suggest improvements, feel free to open an issue or a pull request in the repository.</p>

<h2>License</h2>
<p>This project is licensed under the MIT License. See the <a href="https://github.com/your-username/c-formatter-42/blob/main/LICENSE">LICENSE</a> file for more details.</p>

