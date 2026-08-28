# Desafio — Workflows Automatizados com AWS Step Functions

## Sobre o desafio

Este repositório reúne minhas anotações e aprendizados do laboratório **Explorando Workflows Automatizados com AWS Step Functions**.

O objetivo desta atividade é documentar os conceitos estudados, a experiência prática e os principais insights sobre a construção de workflows automatizados na AWS.

## Objetivos de aprendizagem

* Aplicar os conceitos estudados em um ambiente prático.
* Documentar processos técnicos de forma clara e estruturada.
* Utilizar o GitHub para compartilhar documentação técnica.
## Conceitos principais

### AWS Step Functions

O AWS Step Functions é um serviço de orquestração que permite organizar tarefas em uma sequência lógica e automatizada. Os workflows são representados visualmente, o que facilita entender cada etapa da execução.

### Máquinas de estado

Uma máquina de estado descreve o fluxo de execução de uma aplicação. Ela define qual etapa será executada primeiro, quais condições podem mudar o caminho do fluxo e como o processo será concluído.

### Estados utilizados em workflows

Alguns estados importantes em uma máquina de estado são:

- **Task:** executa uma tarefa, como chamar outro serviço da AWS.
- **Choice:** cria decisões condicionais no workflow.
- **Pass:** repassa dados para a próxima etapa.
- **Wait:** pausa a execução por um período definido.
- **Succeed:** finaliza o workflow com sucesso.
- **Fail:** encerra o workflow quando ocorre uma falha.

### Tratamento de erros
Os workflows podem ser preparados para lidar com falhas. Recursos como `Retry` permitem tentar novamente uma etapa que apresentou erro, enquanto `Catch` direciona a execução para um caminho alternativo de tratamento.
## Aplicação prática

Durante a prática, compreendi como uma máquina de estado pode organizar etapas de um processo automatizado. Cada etapa possui uma função específica, e o fluxo permite visualizar a sequência de execução de forma clara.

Um workflow pode ser estruturado da seguinte forma:

1. Definir a entrada inicial do processo.
2. Executar as tarefas necessárias.
3. Avaliar condições para decidir o próximo caminho.
4. Tratar possíveis erros.
5. Finalizar a execução com sucesso ou registrar uma falha.

## Insights adquiridos

- A representação visual facilita a compreensão e a manutenção dos workflows.
- O tratamento de erros torna os processos mais confiáveis.
- A separação entre as etapas do fluxo deixa a automação mais organizada.
- O histórico de execução ajuda a acompanhar resultados e identificar problemas.

