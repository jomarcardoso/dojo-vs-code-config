# VS Code

Configurações, dicas, atalhos, extensões para te animar e aumentar tua produtividade.

## Formatadores

```json
{
  // ###########################################################################
  // ###################   FORMATADOR DEFAULT - BASE   #########################
  // ###########################################################################

  // formata ao salvar
  "editor.formatOnSave": true,

  // adiciona linha guia na direita
  "editor.rulers": [80],
  "editor.detectIndentation": false,

  // tabulação de 2 espaços
  "editor.tabSize": 2,

  // remove espaços que não devem ser commitados
  "files.trimTrailingWhitespace": true,
  // seleção de texto com 2 cliques ou control
  "editor.wordSeparators": "`~!@#%^&*()-=+[{]}\\|;:'\",.<>/?",

  // insere uma linha no final do arquivo
  "files.insertFinalNewline": true,
}
```

### Melhorias para JS

```json
{
  // ###########################################################################
  // ###################   FORMATADOR DEFAULT - JS/TS   ########################
  // ###########################################################################

  // ponto e vírgula ao final de cada linha
  "javascript.format.semicolons": "insert",
  "typescript.format.semicolons": "insert",

  // aspas simples
  "javascript.preferences.quoteStyle": "single",
  "typescript.preferences.quoteStyle": "single",

  // espaço entre chaves vazias
  "javascript.format.insertSpaceAfterOpeningAndBeforeClosingEmptyBraces": false,
  "typescript.format.insertSpaceAfterOpeningAndBeforeClosingEmptyBraces": false,

  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "typescript": "typescriptreact"
  },

  "emmet.syntaxProfiles": {
    "javascript": "jsx",
    "javascriptreact": "jsx",
    "typescript": "jsx",
    "typescriptreact": "jsx"
  },
  
  "[typescript]": {
    "editor.defaultFormatter": "vscode.typescript-language-features"
  }
}
```

### Melhorias para HTML

```json
{
  // ###########################################################################
  // ###################   FORMATADOR DEFAULT - HTML   #########################
  // ###########################################################################

  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  },

  "html.format.wrapLineLength": 80,
  // quebra a linha de uma forma inteligente

  // quebra os atributos quando há mais do que 1
  "html.format.wrapAttributes": "force-expand-multiline"
}
```

### Melhorias para CSS

```json
{
  // ###########################################################################
  // #################   FORMATADOR DEFAULT - SCSS/CSS   #######################
  // ###########################################################################

  "[scss]": {
    "editor.defaultFormatter": "vscode.css-language-features",
    "editor.wordSeparators": "`~!@#%^*()-=+[{]}\\|;:'\",.<>/?"
  },

  "[css]": {
    "editor.defaultFormatter": "vscode.css-language-features",
    "editor.wordSeparators": "`~!@#%^*()-=+[{]}\\|;:'\",.<>/?"
  }
}
```

## Linter

```json
{
  // ###########################################################################
  // ###################   LINT DEFAULT - SCSS/CSS   ###########################
  // ###########################################################################

  // avisa para evitar !important
  "css.lint.important": "warning",
  "scss.lint.important": "warning",

  // quando for zero, não usar unidade de valor
  "css.lint.zeroUnits": "warning",
  "scss.lint.zeroUnits": "warning",

  // avisa atributos duplicados
  "css.lint.duplicateProperties": "warning",
  "scss.lint.duplicateProperties": "warning",

  // evitar usar float
  "css.lint.float": "warning",
  "scss.lint.float": "warning",

  // evitar seletor de id
  "css.lint.idSelector": "warning",
  "scss.lint.idSelector": "warning"
}
```

## Terminal

```json
{
  // ###########################################################################
  // ###########################   TERMINAL   ##################################
  // ###########################################################################

  "terminal.integrated.profiles.osx": {
    "bash": {
      "path": "C:\\Program Files\\Git\\bin\\bash.exe"
    }
  },
  "terminal.external.windowsExec": "C:\\Program Files\\Git\\bin\\bash.exe",
  "terminal.integrated.defaultProfile.windows": "Git Bash"
}
```

## Git

```
$ git config --global core.editor "code --wait"
```

```json
{
  // ###########################################################################
  // ##############################   GIT   ####################################
  // ###########################################################################
  "git.confirmSync": false,
  "git.autofetch": true,
  "diffEditor.ignoreTrimWhitespace": false
}
```

### Busca

```json
{
  // ###########################################################################
  // #############################   BUSCA   ###################################
  // ###########################################################################
  "search.exclude": {
    "**/*.snap": true,
    "**/dist": true,
    "**/node_modules": true,
    "**/yarn.lock": true,
    "yarn.lock": true,
    "**/package-lock.json": true,
    "package-lock.json": true
  }
}
```

### Estilo

Instalar Fira Code. https://github.com/tonsky/FiraCode

```json
{
  // ###########################################################################
  // ############################   ESTILO   ###################################
  // ###########################################################################

  "editor.fontFamily": "'Fira Code', Consolas, 'Courier New', monospace",
  "editor.fontSize": 13,
  "editor.fontLigatures": true,
  "terminal.integrated.fontSize": 12,
}
```

### Outros

```json
{
  // ###########################################################################
  // ############################   OUTROS   ###################################
  // ###########################################################################

  "explorer.confirmDelete": false
}
```

## Atalhos

- F2 - renomeia
- CTRL + D - seleciona outro com mesmo valor
- ALT + SETA PARA CIMA/BAIXO - move a linha
- ALT + SHIFT + SETA PARA CIMA/BAIXO - copia a linha
- CTRL + X - remove a linha
- CTRL + G - ir para linha
- CTRL + : - comenta linhas selecionadas
- CTRL + p - abre terminal para abrir arquivos ou configs (>)
- ALT + SHIFT + F - formatar arquivo

## Extensões

### GitHub Copilot

![image](https://user-images.githubusercontent.com/27368585/171063760-557d9ff0-1ab0-4573-90ca-148712b68b5f.png)

### LiveServer

![image](https://user-images.githubusercontent.com/27368585/171063930-8c6d5f54-08a0-4631-922b-c1245f880dfa.png)

### Prettier

![image](https://user-images.githubusercontent.com/27368585/171063991-259cd124-8eba-4c89-a658-7089300f247d.png)
