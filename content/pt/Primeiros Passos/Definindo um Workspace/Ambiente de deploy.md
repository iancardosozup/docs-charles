---
title: Ambiente de deploy
weight: 24
description: Nesta seção, você encontra como funciona o ambiente de deploy no Charles.
---

---
 
 O módulo de deploy aplica e monitora os recursos no cluster. E para fazer isso, ele utiliza o padrão [**Operator**](https://kubernetes.io/docs/concepts/extend-kubernetes/operator) que realiza os ciclos de reconciliação garantindo que o cluster sempre estará no estado que você precisa. Os logs do Kubernetes também serão coletados em tempo real.

 ## **Configurando o workspace**
Ao configurar seu workspace é preciso cadastrar as credenciais de acesso ao cluster [**Kubernetes**](https://kubernetes.io/). Essas configurações são específicas para cada uma das ferramentas de _Continuous Deployment_ \(CD\) que são integradas ao CharlesCD. No momento, o Charles realiza o deploy nativamente ou você pode integrar com o [**Spinnaker**](https://www.spinnaker.io/). 

## **Configuração de Deployment**

O Charles possui uma arquitetura adaptável a diferentes instalações Kubernetes. O único requisito é que seu módulo de deploy esteja instalado no cluster de destino com uma URL acessível. A configuração de deployment indica qual é essa URL e quais credenciais do Git serão utilizadas para buscar os charts helm. Sem esta configuração o Charles não conseguirá realizar deploys.

### **Como cadastrar a configuração?**

Siga os passos abaixo:

1. Em **Workspaces,** no menu lateral esquerdo, selecione o workspace desejado, em seguida selecione **Settings ;**
2. Clique em **Credentials;**
3. Clique em **Add Deployment Configuration;**

Preencha os seguintes campos:

1. **Butler URL:** URL do módulo de deploy Butler. Caso este esteja no mesmo cluster de instalação do Charles, utilize seu FQDN \(Fully Qualified Domain Name\). Exemplo: `http://charlescd-butler.butler-namespace.svc.cluster.local:3000`.
2. **Namespace:** Defina o namespace em que os recursos serão disponibilizados no cluster. Você deve criar o seu namespace, uma vez que o Charles não faz isso;
3. **Git provider:** Defina o provedor de git a ser utilizado \(**GitHub** ou **GitLab**\);
4. **Git token:** Insira um token de autenticação que tenha acesso repositório git onde está armazenado seus [**templates Helm**]({{< ref path="/Primeiros Passos/Criando seu primeiro módulo/Configurando o chart template.md" lang="pt">}}) que serão utilizados durante o deployment da sua [**aplicação**]({{< ref path="/Primeiros Passos/Criando seu primeiro módulo/Visao geral.md" lang="pt">}}). Caso o seu Git Provider seja **GitHub**, é necessário a permissão "_repo_". Se não, configure no **GitLab** os acessos: "_api_ " e "_read\_repository_". 

{{% alert color="info" %}}
To avoid dependency of a specific user in the authentication token field, use [**Machine Account**](https://docs.github.com/en/developers/overview/managing-deploy-keys#machine-users). 
{{% /alert %}}
 
