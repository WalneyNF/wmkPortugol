wmkPortugol

 

wmkPortugol é um editor online de código Portugol que permite escrever programas em Portugol e convertê-los automaticamente para outras linguagens de programação, como JavaScript, Python, C, Java, PHP, Lua, GDScript (Godot Engine), GameMaker Language (GML) e muito mais! Este projeto foi criado para facilitar o aprendizado de programação e ajudar desenvolvedores a migrar seus códigos iniciais para linguagens mais avançadas.

O editor é totalmente open-source, permitindo que qualquer pessoa contribua com melhorias, adicione novas linguagens ou ajuste os mapeamentos existentes.

Índice

Sobre o Projeto

Funcionalidades

Como Usar

Como Contribuir

Adicionando Novas Linguagens

Estrutura dos Arquivos JSON

Licença

Créditos

Contato

Sobre o Projeto

O wmkPortugol foi desenvolvido para ajudar estudantes, professores e desenvolvedores a aprenderem lógica de programação usando a linguagem Portugol, uma linguagem simples e intuitiva baseada no português. Além disso, o editor oferece uma funcionalidade única: a conversão automática de código Portugol para várias linguagens de programação.

Público-alvo:

Estudantes: Aprender conceitos básicos de programação sem se preocupar com a sintaxe complexa de linguagens avançadas.

Professores: Criar exemplos de código em Portugol e convertê-los para linguagens usadas no mercado de trabalho.

Desenvolvedores: Migrar rapidamente ideias iniciais escritas em Portugol para linguagens específicas.

Funcionalidades

Editor Online: Escreva código Portugol diretamente no navegador.

Execução Simples: Execute o código Portugol e veja a saída no painel de resultados.

Conversão Multi-Linguagem: Converta código Portugol para várias linguagens de programação.

Tema Escuro/Claro: Alterne entre modos claro e escuro para maior conforto visual.

Menus Intuitivos: Acesse opções como "Novo", "Abrir", "Salvar" e "Converter" através de menus organizados.

Extensível: Adicione suporte a novas linguagens facilmente editando arquivos JSON.

Como Usar

Executar Localmente

Clone o repositório:

git clone https://github.com/WalneyNF/wmkPortugol.git

Abra o arquivo index.html no seu navegador.

Basta abrir o arquivo diretamente ou usar um servidor local (como Live Server no VS Code).

Escreva seu código Portugol na área de edição e clique em "Executar" para ver a saída.

Para converter o código, clique no menu "Conversão" e escolha a linguagem desejada.

Exemplo de Uso

Código Portugol:

escreva("Olá, mundo!")
leia(x)
para i de 1 ate 5 faca
    escreva(i)
fimpara

Resultado em Python:

print("Olá, mundo!")
x = input("Digite um valor para x: ")
for i in range(1, 6):
    print(i)

Como Contribuir

Contribuições são bem-vindas! Para colaborar:

Fork o Repositório

Clique no botão "Fork" no GitHub para criar uma cópia do projeto na sua conta.

Clone o Repositório Forkado

git clone https://github.com/seu-usuario/wmkPortugol.git

Faça Suas Alterações

Corrija bugs, melhore a interface ou adicione novas funcionalidades.

Envie um Pull Request

Após testar suas alterações, envie um pull request explicando suas mudanças.

Adicionando Novas Linguagens

Criar um Novo Arquivo JSON

Crie um novo arquivo JSON no diretório /json com o nome da linguagem (ex.: ruby.json, go.json).

Estrutura do Arquivo JSON:

{
    "escreva": "print($1)",
    "leia": "$1 = input()",
    "para": "for $1 in range($2, $3 + 1):",
    "fimpara": "",
    "se": "if $1:",
    "fimse": "",
    "<-": "$1 = $2"
}

Atualizar o Menu de Conversão

Adicione uma nova opção no submenu "Conversão" no arquivo index.html:

<button onclick="converterCodigo('ruby')">Ruby</button>

Testar

Escreva código Portugol no editor, converta para a nova linguagem e verifique se a saída está correta.

Licença

Este projeto está licenciado sob a MIT License, permitindo o uso, modificação e distribuição livre, desde que os créditos originais sejam mantidos.

Créditos

Autor: Walney Moreira Klein

Colaboradores: Lista de Colaboradores

Contato

Email: walneyk@hotmail.com

GitHub: @WalneyNF

Repositório: wmkPortugol

