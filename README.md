# Missão Suporte Vital

![Python](https://img.shields.io/badge/Python-3.6%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Git](https://img.shields.io/badge/Git-Versionamento-orange?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-Repositório-black?style=for-the-badge&logo=github&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen?style=for-the-badge)

Projeto desenvolvido para a disciplina de **Gestão e Qualidade de Software**, com foco na prática de um fluxo de desenvolvimento corporativo utilizando **Git e GitHub**.

A atividade simula a implementação de um **módulo de monitoramento de suporte à vida em uma estação espacial**, utilizando um processo de entrega organizado em diferentes ambientes: **desenvolvimento, homologação e produção**.

Além da implementação do módulo, o principal objetivo da atividade é compreender como as alterações podem percorrer diferentes etapas de validação antes de serem disponibilizadas na versão final do sistema.

## ▸ Conceito da atividade

A atividade consiste na criação de um repositório chamado `estacao-espacial-orbit` e na implementação de um módulo responsável pelo monitoramento dos parâmetros essenciais de suporte à vida da estação espacial.

O projeto foi estruturado seguindo um fluxo de branches em três camadas:

```text
develop
   ↓
stage
   ↓
main
```

Cada branch possui uma responsabilidade específica dentro do processo de desenvolvimento.

As alterações são inicialmente implementadas na branch `develop`. Após a validação do código, elas são promovidas para `stage`, onde ocorre a etapa de homologação. Por fim, depois da aprovação final, a implementação é integrada à branch `main`, representando a versão de produção.

Esse fluxo simula uma estrutura utilizada em ambientes corporativos para aumentar a organização, a segurança e a confiabilidade das entregas.

## ▸ Camadas do ambiente

### `develop` - Desenvolvimento

A branch `develop` representa o ambiente destinado à implementação das novas funcionalidades.

Neste ambiente são realizadas:

- Criação e alteração do código;
- Desenvolvimento do módulo de suporte à vida;
- Correções e melhorias;
- Testes iniciais das funcionalidades.

É a primeira etapa do fluxo de entrega e onde as alterações permanecem antes de serem encaminhadas para homologação.

### `stage` - Homologação

A branch `stage` representa o ambiente de **testes e validação**.

Após o desenvolvimento, as alterações da `develop` são enviadas para essa branch através de um **Pull Request**.

Nesta etapa ocorre:

- Revisão das alterações realizadas;
- Validação das funcionalidades;
- Simulação do processo de Code Review;
- Aprovação antes da implantação em produção.

A `stage` funciona como uma camada intermediária de segurança entre o desenvolvimento e a versão final do sistema.

### 🚀 `main` - Produção

A branch `main` representa a versão oficial e estável do projeto.

Somente alterações que passaram pelas etapas de desenvolvimento e homologação devem chegar a essa branch.

O fluxo de lançamento ocorre da seguinte forma:

```text
develop → stage → main
```

Dessa forma, a versão principal do projeto permanece mais organizada e confiável.

## ▸ Fluxo de Pull Requests

Durante a atividade, foram realizados dois processos de promoção de código utilizando **Pull Requests**.

### 1. Desenvolvimento para Homologação

```text
develop → stage
```

Nesta etapa, o módulo desenvolvido é encaminhado para validação.

**Pull Request:**

```text
[Stage] feat: Módulo de Suporte de Vida
```

Antes do merge, são realizadas a revisão e a aprovação das alterações.

### 2. Homologação para Produção

```text
stage → main
```

Após a validação na `stage`, o código é promovido para a versão oficial.

**Pull Request:**

```text
[Release v1.0] Implantação do Módulo de Suporte de Vida
```

Esse processo representa a liberação da funcionalidade para o ambiente de produção.

## ▸ Módulo de Suporte Vital

O sistema desenvolvido é responsável por representar o monitoramento dos principais parâmetros relacionados ao suporte à vida da estação espacial.

O módulo possui uma função responsável por verificar os níveis do ambiente e informar o status dos sistemas essenciais.

Entre os elementos monitorados estão parâmetros críticos para a segurança e o funcionamento da missão.

O objetivo da implementação é demonstrar, por meio de um algoritmo simples, como um sistema pode centralizar informações importantes sobre o funcionamento de componentes essenciais.

## ▸ Versionamento e qualidade de software

A atividade foi desenvolvida com foco na aplicação prática de conceitos relacionados ao **versionamento de código** e à **organização do processo de entrega de software**.

Durante o desenvolvimento, foram utilizados conceitos importantes:

| Conceito             | Aplicação no projeto                                 |
| -------------------- | ---------------------------------------------------- |
| **Repositório**      | Armazenamento do código e documentação do projeto    |
| **Branch `develop`** | Desenvolvimento das funcionalidades                  |
| **Branch `stage`**   | Homologação e validação das alterações               |
| **Branch `main`**    | Versão estável e oficial do projeto                  |
| **Commit**           | Registro das alterações realizadas                   |
| **Push**             | Envio das alterações para o repositório remoto       |
| **Pull Request**     | Solicitação para promover alterações entre ambientes |
| **Code Review**      | Revisão das alterações antes da aprovação            |
| **Merge**            | Integração das alterações entre as branches          |

A utilização dessas práticas permite acompanhar a evolução do projeto e organizar melhor o ciclo de desenvolvimento.

## ▸ Fluxo de desenvolvimento

O processo seguido na atividade pode ser representado da seguinte forma:

```text
1. Criar repositório
        ↓
2. Criar branch stage
        ↓
3. Criar branch develop
        ↓
4. Desenvolver módulo
        ↓
5. Commit e Push
        ↓
6. Pull Request: develop → stage
        ↓
7. Revisão e Homologação
        ↓
8. Pull Request: stage → main
        ↓
9. Aprovação final
        ↓
10. Merge para produção
```

Esse fluxo demonstra como uma alteração pode passar por diferentes níveis de validação antes de chegar à versão principal.

## ▸ Como executar

**Pré-requisito:** possuir a linguagem utilizada no desenvolvimento instalada na máquina.

1. Clone o repositório:

```bash
git clone https://github.com/miguelalchaar/estacao-espacial-orbit.git
```

2. Acesse a pasta do projeto:

```bash
cd estacao-espacial-orbit
```

3. Execute o arquivo do módulo de suporte à vida de acordo com a linguagem utilizada no projeto.

Exemplo em python:

```bash
python suporte-vida.py
```

## ▸ Autor

Projeto desenvolvido pelos responsáveis pela implementação e manutenção do módulo da missão:

- **miguelalchaar** - Desenvolvedor
