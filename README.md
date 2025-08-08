# 🧾 Suíte de Testes - Filtro "Concluidos (Completed)"
Este repositório faz parte do meu aprendizado em QA, onde documento a criação de suítes de teste usando critérios de aceite escritos em Gherkin. O objetivo aqui é desenvolver uma visão crítica para validar funcionalidades com clareza e organização, preparando um material que facilite análise e automação.

O foco é aprimorar a escrita técnica, simular cenários reais de teste e mostrar a importância de uma suíte de testes bem construída para garantir qualidade.

**Site utilizado nos testes:** [TodoMVC - React](https://todomvc.com/examples/react/dist/) 

<details>
  <summary><strong>📋 Clique aqui para ver a suíte de testes</strong></summary>

<br>

<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Cenário</th>
      <th>Caso de Teste (Gherkin)</th>
      <th>Prioridade</th>
      <th>Severidade</th>
      <th>Resultado Esperado</th>
      <th>Resultado Obtido</th>
      <th>Defeitos</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CT01</td>
      <td>Exibir apenas itens concluídos</td>
      <td>Dado que possuo itens pendentes e concluídos<br>Quando clico no filtro "Completed"<br>Então apenas os itens concluídos devem ser exibidos</td>
      <td>Alta</td>
      <td>Alta</td>
      <td>Apenas os itens concluídos devem ser exibidos</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
    <tr>
      <td>CT02</td>
      <td>Ocultar itens pendentes</td>
      <td>Dado que tenho ao menos um item pendente<br>Quando clico no filtro "Completed"<br>Então os itens pendentes não devem ser exibidos na lista</td>
      <td>Média</td>
      <td>Alta</td>
      <td>Itens pendentes não são exibidos na lista</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
    <tr>
      <td>CT03</td>
      <td>Itens concluídos com checkbox marcado</td>
      <td>Dado que existem itens concluídos<br>Quando clico no filtro "Completed"<br>Então os itens devem aparecer com checkbox marcado e texto riscado</td>
      <td>Baixa</td>
      <td>Média</td>
      <td>Checkbox marcado e texto riscado para itens concluídos</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
    <tr>
      <td>CT04</td>
      <td>Contador mostra itens pendentes corretamente</td>
      <td>Dado que existem 5 itens na lista<br>E 2 desses itens estão concluídos<br>Quando seleciono o filtro "Completed"<br>Então a lista exibe os 2 itens concluídos<br>E o contador exibe "3 items left"</td>
      <td>Média</td>
      <td>Média</td>
      <td>Exibir 2 itens concluídos e contador com "3 items left"</td>
      <td>Passou conforme esperado</td>
      <td>—</td>
      <td>Concluído</td>
    </tr>
  </tbody>
</table>
</details>


## 🧪 O que é uma Suíte de Testes?

Uma suíte de testes reúne casos que validam o comportamento esperado de uma funcionalidade ou fluxo, assegurando que a aplicação funcione conforme o planejado e que possíveis falhas sejam detectadas rapidamente.

 Ter uma suíte bem documentada é essencial para:
- Cobrir os principais cenários e variações
- Facilitar a execução manual e futura automação
- Ajudar na rastreabilidade dos testes
- Manter consistência na validação de funcionalidades
- Apoiar entregas com mais confiança

---

## ✍️ Linguagem Gherkin
A linguagem Gherkin é usada para escrever casos de teste de forma simples e legível, mesmo por pessoas não técnicas.
Ela segue o formato:

```
Cenário: [descrição do cenário]  
Dado que [estado inicial]  
Quando [ação realizada]  
Então [resultado esperado]  
```
---

Esse formato facilita a comunicação entre desenvolvedores, QAs e stakeholders, pois descreve o comportamento do sistema pela ótica do usuário.

---

## 📝 User Story  
Eu, como usuária da aplicação  
Gostaria de visualizar apenas os itens concluídos da minha lista  
Porque assim posso verificar rapidamente o que já foi finalizado

---

## 📌 Regras de Negócio

- **RN1**: O filtro "Completed" exibe apenas os itens concluídos
- **RN2**: Itens concluídos aparecem com texto riscado e checkbox marcado
- **RN3**: Itens pendentes devem ser ocultados nessa visualização
- **RN4**: O contador permanece visível e reflete corretamente a quantidade de itens pendentes

---

## ✅ Critérios de Aceite (Gherkin)  
**Cenário:** Visualizar apenas os itens concluídos com o filtro "Completed"<br>
**Dado que** existam itens pendentes e concluídos na lista<br>
**Quando** seleciono o filtro "Completed"<br>
**Então** somente os itens concluídos devem ser exibidos na lista<br>
**E** eles devem aparecer com checkbox marcado e texto riscado<br>
**E** o contador no rodapé deve exibir a quantidade correta de itens pendentes

---

## 🧠 Diferença entre Prioridade e Severidade

| Conceito       | O que significa                                                        | Quem define          |
| -------------- | ---------------------------------------------------------------------- | -------------------- |
| **Prioridade** | Define o quão rápido o teste deve ser executado ou o defeito resolvido | Time de produto / QA |
| **Severidade** | Mede o impacto técnico do problema no sistema                          | Time de QA           |

---

## 📝 Sobre os Casos de Teste
Todos os testes foram escritos com foco em:

- Cobrir os comportamentos principais do filtro "Completed"
- Trabalhar com critérios claros e mensuráveis
- Organizar os testes com colunas como Prioridade, Severidade, Status, etc.

  ---

  🎯 Objetivo do Projeto
 Praticar a criação de suítes de testes a partir de critérios bem definidos.

- Validar o comportamento do filtro "Concluídos (Completed)" na exibição dos itens
- Reforçar o uso de Gherkin como ponte entre negócio e testes
- Desenvolver habilidades práticas essenciais para a atuação em QA

---

## 📌 Observação
Este projeto não contém código-fonte, pois o foco está na documentação de testes e raciocínio analítico em QA.
É um exercício essencial para fortalecer a base teórica e desenvolver uma visão crítica sobre o que deve ser testado em uma aplicação.

























