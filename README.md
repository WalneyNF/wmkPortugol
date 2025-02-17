# **wmkPortugol**
![wmkPortugol](https://img.shields.io/badge/Status-Ativo-brightgreen) ![License-MIT](https://img.shields.io/badge/License-MIT-blue)

**wmkPortugol** é um editor online de código Portugol que permite escrever programas em Portugol e convertê-los automaticamente para outras linguagens de programação, como JavaScript, Python, C, Java, PHP, Lua, GDScript (Godot Engine), GameMaker Language (GML) e muito mais! Este projeto foi criado para facilitar o aprendizado de programação e ajudar desenvolvedores a migrar seus códigos iniciais para linguagens mais avançadas.

O editor é totalmente **open-source**, permitindo que qualquer pessoa contribua com melhorias, adicione novas linguagens ou ajuste os mapeamentos existentes.
---

## **Índice**

1. [Sobre o Projeto](#sobre-o-projeto)
2. [Funcionalidades](#funcionalidades)
3. [Como Usar](#como-usar)
4. [Como Contribuir](#como-contribuir)
5. [Adicionando Novas Linguagens](#adicionando-novas-linguagens)
6. [Estrutura dos Arquivos JSON](#estrutura-dos-arquivos-json)
7. [Licença](#licença)

---

## **Sobre o Projeto**

O **wmkPortugol** foi desenvolvido para ajudar estudantes, professores e desenvolvedores a aprenderem lógica de programação usando a linguagem Portugol, uma linguagem simples e intuitiva baseada no português. Além disso, o editor oferece uma funcionalidade única: a conversão automática de código Portugol para várias linguagens de programação.

Isso é especialmente útil para:

- **Estudantes**: Aprender conceitos básicos de programação sem se preocupar com a sintaxe complexa de linguagens avançadas.
- **Professores**: Criar exemplos de código em Portugol e convertê-los para linguagens usadas no mercado de trabalho.
- **Desenvolvedores**: Migrar rapidamente ideias iniciais escritas em Portugol para linguagens específicas.

---

## **Funcionalidades**

- **Editor Online**: Escreva código Portugol diretamente no navegador.
- **Execução Simples**: Execute o código Portugol e veja a saída no painel de resultados.
- **Conversão Multi-Linguagem**: Converta código Portugol para várias linguagens de programação.
- **Tema Escuro/Claro**: Alterne entre modos claro e escuro para maior conforto visual.
- **Menus Intuitivos**: Acesse opções como "Novo", "Abrir", "Salvar" e "Converter" através de menus organizados.
- **Extensível**: Adicione suporte a novas linguagens facilmente editando arquivos JSON.

---

## **Como Usar**

### 1. **Executar Localmente**
Para usar o **wmkPortugol**, siga os passos abaixo:

1. Clone o repositório:
   ```bash
   git clone https://github.com/WalneyNF/wmkPortugol.git

2. Abra o arquivo `index.html` no seu navegador:
   - Basta abrir o arquivo diretamente ou usar um servidor local (como Live Server no VS Code).

3. Escreva seu código Portugol na área de edição e clique em "Executar" para ver a saída.

4. Para converter o código, clique no menu **"Conversão"** e escolha a linguagem desejada.

---

### 2. **Exemplo de Uso**

#### Código Portugol:
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
Contribuições são bem-vindas! Se você deseja melhorar o wmkPortugol , siga estas etapas:

Fork o Repositório :
1. Clique no botão "Fork" no GitHub para criar uma cópia do projeto na sua conta.
2. Clone o Repositório Forkado :
   git clone https://github.com/WalneyNF/wmkPortugol.git

3. Faça Suas Alterações :
   Corrija bugs, melhore a interface ou adicione novas funcionalidades.
4. Envie um Pull Request :
   Após testar suas alterações, envie um pull request explicando suas mudanças.

Adicionando Novas Linguagens

O wmkPortugol foi projetado para ser altamente extensível. Você pode adicionar suporte a novas linguagens seguindo estes passos:

1. Criar um Novo Arquivo JSON
Crie um novo arquivo JSON no diretório /json com o nome da linguagem (ex.: ruby.json, go.json). O arquivo deve seguir o padrão abaixo:

{
    "escreva": "COMANDO_EQUIVALENTE",
    "leia": "COMANDO_EQUIVALENTE",
    "para": "COMANDO_EQUIVALENTE",
    "fimpara": "COMANDO_EQUIVALENTE",
    "se": "COMANDO_EQUIVALENTE",
    "fimse": "COMANDO_EQUIVALENTE",
    "<-": "COMANDO_EQUIVALENTE"
}

2. Atualizar o Menu de Conversão
Adicione uma nova opção no submenu "Conversão" no arquivo index.html:

<button onclick="converterCodigo('ruby')">Ruby</button>

3. Testar
Escreva código Portugol no editor, converta para a nova linguagem e verifique se a saída está correta.

Estrutura dos Arquivos JSON
Os arquivos JSON devem conter mapeamentos para os seguintes comandos básicos do Portugol:

## **Estrutura dos Arquivos JSON**

Os arquivos JSON devem conter mapeamentos para os seguintes comandos básicos do Portugol:

| Comando Portugol | Descrição                                | Exemplo de Mapeamento (Python)       |
|-------------------|------------------------------------------|---------------------------------------|
| `escreva`         | Exibe mensagens na tela                 | `"print"`                            |
| `leia`            | Lê entrada do usuário                   | `"$1 = input('Digite um valor para $1: ')` |
| `para`            | Loop `for`                              | `"for $1 in range($2, $3 + 1):"`     |
| `fimpara`         | Finaliza o loop `for`                   | `""`                                 |
| `se`              | Condição `if`                           | `"if $1:"`                           |
| `fimse`           | Finaliza a condição `if`                | `""`                                 |
| `<-`              | Operador de atribuição                  | `"$1 = $2"`                          |

Use placeholders (`$1`, `$2`, `$3`) para representar variáveis ou valores dinâmicos.

---

## **Licença**

Este projeto está licenciado sob a **MIT License**, o que significa que você pode usá-lo, modificá-lo e distribuí-lo livremente, desde que mantenha os créditos originais.

---

## **Créditos**

- **Autor**: [Walney Moreira Klein](https://github.com/WalneyNF)
- **Colaboradores**: [Lista de Colaboradores](https://github.com/WalneyNF/wmkPortugol/graphs/contributors)

---

## **Contato**

Se tiver dúvidas, sugestões ou quiser colaborar, entre em contato:

- Email: walneyk@hotmail.com
- GitHub: [@WalneyNF](https://github.com/WalneyNF)

https://github.com/WalneyNF/wmkPortugol

