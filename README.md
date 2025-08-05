# 🚀 Ansible Nginx Setup

Este projeto demonstra como automatizar a configuração de um servidor **Nginx** utilizando **Ansible**, de forma simples e eficiente.

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

## 🧠 Sobre

**Automação básica** com **Ansible** para provisionar um servidor web **Nginx**. Ideal para **aprendizado** ou **primeiros** testes em DevOps.

## Créditos

Automação de configuração com Ansible 🚀
