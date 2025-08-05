# 🚀 Ansible Nginx Setup

## Projeto Gerenciamento de Configuração com Ansible

Este projeto foi desenvolvido como parte de um desafio prático de DevOps, com o objetivo de resolver problemas de **consistência**, **segurança** e **eficiência** na configuração de servidores em uma empresa fictícia de e-commerce.

A situação simulada envolve uma infraestrutura mista (on-premises e cloud), que vinha sendo configurada manualmente, gerando falhas e vulnerabilidades. Para resolver isso, foi adotada uma solução de **gerenciamento de configuração com Ansible**, automatizando a instalação e configuração do servidor web Nginx.

Este projeto representa uma **estratégia prática** para garantir que todos os servidores mantenham configurações padronizadas e seguras, reduzindo erros humanos e otimizando o tempo da equipe de TI..

## 📁 Estrutura do Projeto

```
ansible-nginx-setup/
├── README.md
├── hosts.ini
├── nginx_setup.yml
├── img/
│   ├── teste_nginx.PNG
└── files/
    ├── nginx.conf
    └── index.html
```

## ⚙️ Pré-requisitos

- **Ansible** instalado no seu sistema (ex: **WSL** no **Windows** no meu caso)
- **Servidores** com **SSH acessível** ou uso de `localhost`
- **Acesso** com permissões de **sudo**(`--ask-become-pass`)

## 🧪 Como usar

1. **Edite** o arquivo `hosts.ini` com os **IPs** dos seus **servidores** (ou use `localhost`);
2. Execute o **playbook** com o seguinte comando:

```bash
ansible-playbook -i hosts.ini nginx_setup.yml --ask-become-pass
```

3. Acesse o **servidor** via **navegador**:
   `http://localhost`

Se tudo estiver certo, verá a seguinte tela:

![Serviodor Nginx Funcionando](/img/teste_nginx.PNG)

## 🛠️ Ferramentas Utilizadas

- Ansible

- Nginx

- WSL (Ubuntu)

- Git / GitHub

## 🧠 Sobre

**Automação básica** com **Ansible** para provisionar um servidor web **Nginx**. Ideal para **aprendizado** ou **primeiros** testes em DevOps.

## Créditos

Automação de configuração com Ansible 🚀
Desafio de DevOps — Projeto de gerenciamento de configuração.