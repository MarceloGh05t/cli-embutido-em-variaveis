# cli-embutido-em-variaveis
Criei uma metodologia para usar comando cli e código shell através de variáveis do tipo strings.   

Eu atribui o command-line interface (CLI) em formato de string dentro de variáveis.

Estrutura:

```
var nome_variavel = "comando cli";
```

Exemplo:

```
var executa_cli = "start calc.exe";

```

Depois bata salvar o arquivo usando o conteúdo desta variável com a extensão (.bat).

Pode usar esta lógica para vbs e comandos shell. Depois você salva o contéudo desta variável como uma extensão bat, vbs ou outras que usam cli ou shell,
permitindo que a aplicação possa criar e executar arquivos, que sem permissão podem ser barrados por antivírus.

Exemplo, que irá abrir um arquivo teste.bat sem abrir a janela cmd (tela preta):

```
var executa_bat = "Set WshShell = CreateObject(""WScript.Shell"")
WshShell.Run ""teste.bat"", 0";
```
Depois bata salvar o arquivo usando o conteúdo desta variável com a extensão (.vbs).
