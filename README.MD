# Escalonador de processos FIFO

Este projeto simula o algoritimo de escalonamento de processos FIFO, em que os processos são executados de acordo com a ordem de chegada. Além disso, exibe diversas métricas durante e no final da execução dos processos.

## Tabela de Conteúdos
- [Funcionalidades](#funcionalidades)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Descrição dos Arquivos](#descrição-dos-arquivos)
- [Instalação e Execução](#instalação-e-execução)

## Funcionalidades
- **Simulação de Escalonamento**: Implementa o algoritmo FIFO para escalonar os processos.
- **Entrada Personalizável**: Permite ao usuário definir processos com tempos específicos de chegada e execução.
- **Controle do usuário**: Permite não só que o usuário execute os processos passo a passo ou com timer, como também deixa que ele defina a ordem de execução dos processos, caso dois ou mais cheguem ao mesmo tempo.

## Estrutura do Projeto
```bash
processos/
├── cpu_ociosa.csv
├── normal.csv
└── tempo_chegada_igual.csv
cpu.py
main.py
processo.py
util.py
README.md
```

## Descrição dos Arquivos

- **cpu.py**: Contém a implementação da classe CPU, responsável por gerenciar a fila de prontos e o ciclo de execução dos processos.
- **main.py**: Script principal para execução da simulação, com opções de seleção de processos pré-definidos ou inserção manual.
- **processo.py**: Define a classe `Processo` e a classe `Processos`, que manipulam os atributos e armazenamento dos processos.
- **util.py**: Funções utilitárias para auxiliar na limpeza do terminal e exibição de erros.
- **processos/**: Contém arquivos CSV de exemplo com 3 cenários de processos (CPU ociosa, chegada ao mesmo tempo e cpu ativa até o final).

## Pré-requisitos para Execução
- Python versão 3.12.1 ou superior
- Módulo tabulate

## Download e Execução

1. **Clone o repositório**:
    ```bash
    git clone https://github.com/Julielison/Escalonador-de-Processos-FIFO.git
    ```
2. **Baixe as dependências:**
    ```
    pip install tabulate
    ```

2. **Execute o programa**:
    ```bash
    python main.py
    ```
   - Utilize os arquivos CSV de exemplo ou insira processos manualmente.
   - Escolha a execução manual ou automática para acompanhar a simulação dos processos.

Após a execução, os resultados podem ser visualizados diretamente no terminal.