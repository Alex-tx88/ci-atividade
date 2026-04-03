# Documentação do Pipeline de CI - GitHub Actions

## 1. Descrição do projeto
Este projeto consiste na implementação de um pipeline simples de Continuous Integration (CI) utilizando o GitHub Actions. A automação foi configurada para executar comandos básicos no terminal sempre que houver uma atualização no código do repositório.

## 2. Objetivo da atividade
O objetivo desta atividade é desenvolver a habilidade de documentar processos técnicos e configurar um pipeline que execute automaticamente um script ou comando quando ocorrer um evento de push.

## 3. Estrutura do projeto
Os arquivos que compõem este repositório são:
* **.github/workflows/ci.yml**: Arquivo de configuração contendo as instruções de automação do pipeline.
* **README.md**: Este arquivo, contendo a documentação técnica do projeto.

## 4. Explicação do workflow
O arquivo ci.yml está estruturado da seguinte forma:

* **name: CI Example**: Nome do workflow exibido na aba Actions.
* **on: [push]**: Gatilho que inicia o pipeline a cada novo push.
* **jobs**: Define o conjunto de tarefas.
* **runs-on: ubuntu-latest**: Indica que o pipeline roda em uma máquina virtual Ubuntu.
* **steps**: Sequência de passos do trabalho.
* **name: Print message**: Identificador visual do passo.
* **run: echo "Atividade feita com sucesso!"**: Comando que imprime a mensagem no terminal.

## 5. Fluxo do pipeline
O fluxo segue o caminho abaixo:

1. **Push no GitHub**
2. **Execução do pipeline** (Gatilho automático)
3. **Execução do comando** (Impressão da mensagem)
4. **Exibição do resultado** (Status de sucesso na aba Actions)

## 6. Resultado da execução
Ao realizar um push, o GitHub Actions provisiona a máquina virtual e executa os passos definidos. O resultado esperado é que o job apresente um status de sucesso (check verde), exibindo a mensagem personalizada no log do terminal.
