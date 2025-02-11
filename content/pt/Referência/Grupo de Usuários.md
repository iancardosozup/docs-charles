---
title: Grupo de Usuários
weight: 55
description: >-
  Nesta seção, você encontra detalhes sobre como funcionam os Grupos de Usuários
  no Charles.
---

---

Um grupo de usuários pode representar um time ou até mesmo um subconjunto de pessoas baseado em suas habilidades. 

Por exemplo, em um time muito grande, as permissões de acesso ao Charles poderiam se diferenciar de acordo com a posição de seus membros, você teria os seguintes grupos:

* Desenvolvedores do Produto X.
* QAs do Produto X.
* Data Analysts do Produto X.

Porém, se todos do time tiverem a mesma permissão, você pode criar apenas um grupo com todos os usuários:

* Time do Produto X.

![Visualiza&#xE7;&#xE3;o do Grupo de Usu&#xE1;rios &quot;Data Analysts do Produto X&quot;](/shared/image%20%283%29.png)

## **Permissões para o Grupo de Usuários no Workspace**

As permissões do Charles são dadas aos grupos de usuários quando você os associa a um workspace.

Os seguintes perfis são suportados: 

* **Mantenedor**: pode acessar e editar todas as configurações do workspace. Ele pode realizar implantações, e também tem a permissão para criar, editar e deletar círculos e módulos.
* **Desenvolvedor**: possui acesso para realizar implantações e também pode criar, editar, deletar círculos e módulos. 
* **Analista**: pode visualizar módulos. Possui permissão para criar, editar e deletar círculos.
* **Leitor**: pode visualizar círculos e módulos.

![Escolha de permiss&#xE3;o ao associar um grupo de usu&#xE1;rios a um workspace.](/shared/chrome-capture-3-.gif)

### **Mapa de Permissões**

Segue abaixo as permissões vinculadas a cada perfil:

| Módulos | Ação | Maintainer | Developer | Analyst  | Reader |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **Usuários** | Criar  |   |   |   |   |
|   | Editar |   |   |   |   |
|   | Deletar |   |   |   |   |
|   | Visualizar  |   |   |   |   |
| **Grupo de usuários** | Criar |   |   |   |   |
|   | Editar  |   |   |   |   |
|   | Deletar |   |   |   |   |
|   | Visualizar  |   |   |   |   |
| **Workspace** | Criar |   |   |   |   |
|   | Configurar | ✔ |   |   |   |
|   | Deletar |   |   |   |   |
|   | Visualizar | ✔  | ✔  | ✔  | ✔  |
| **Circle** | Criar/Editar/Deletar | ✔  | ✔  | ✔  |   |
|   | Visualizar | ✔  | ✔  | ✔  | ✔  |
| **Modules**  | Criar/Editar/Deletar | ✔  | ✔  |   |   |
|   | Visualizar  | ✔  | ✔  | ✔  | ✔  |
| **Deploy**  | Fazer deployments | ✔  | ✔  |   |   |
