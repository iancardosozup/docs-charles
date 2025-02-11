---
title: Grupo de métricas
weight: 78
description: >-
  Nesta seção, você encontra detalhes sobre como funcionam os grupos de métricas
  no Charles.
---

---

O grupo de métricas é uma funcionalidade que permite você cadastrar e organizar em grupos qualquer tipo de métrica dentro da sua aplicação. Essas métricas são relacionadas com o [**provedor que você cadastrou anteriormente**]({{< ref path="/Primeiros Passos/Definindo um Workspace/Adicionando o Datasource.md" lang="pt">}}). 

### **Como criar um grupo?**

Para criar o seu grupo de métricas, siga os passos abaixo:

**Passo 1:** Vá até em '**Circles'** no menu lateral direito e escolha o circulo que você quer criar um novo grupo de métrica; 

**Passo 2:** Em **Add metrics group,** digite o nome que desejar para o seu grupo e clique em **add group**. 

![](/shared/criacaogroup.gif)

Depois que você criou seu grupo, agora você pode cadastrar a sua métrica:

**Passo 3:** Clique em **Add metric** e coloque o nome da métrica que você deseja;

**Passo 4:** Em **select a data source**, selecione o seu provedor de métrica já cadastrado;

**Passo 5:** Clique em **Metric** e escolha uma métrica e depois disso, utilize o **Filter** para customizar com o valor e a condicional que você precisa. Esse é o campo onde o seu provedor irá retornar as métricas que já existem. 

Veja o exemplo abaixo: 

![](/shared/metric+filter.gif)

**Passo 6:**  Defina um **Threshold** para estabelecer um limite para sua métrica. 

{{% alert color="info" %}}
**Threshold** são limites predeterminados que você pode configurar no Charles. Ele irá informar quando um deles atingir o valor especificado. 

Por exemplo, se você quiser saber quando sua aplicação atingir um limite de 50 erros, basta customizar o **threshold**  para que você seja informado de quando essa métrica for atingida. 
{{% /alert %}}

![](/shared/threshold.gif)

{{% alert color="success" %}}
Pronto! Você cadastrou seu grupo de métricas. 
{{% /alert %}}

Agora acompanhe o resultado com os gráficos e as informações disponíveis. 

![](/shared/graficos.gif)

## **Grupo de Métricas: Advanced** 

Você pode customizar sua própria métrica com a funcão **advanced.** Essa opção é para usuários que já sabem fazer uma query no Datasource que eles estão utilizando, e também oferece o poder de criar qualquer métrica usando essa ferramenta.

Veja o exemplo abaixo_,_ mostra onde usar o **PromQL** para fazer queries no Prometheus, criando um novo tipo de métrica: 

![](/shared/advanced.png)

