# Sintaxe YAML

Exemplos apresentando a sintaxe da linguagem YAML.

## Chave-Valor

```yaml
fruta: banana
vegetal: cenoura
liquido: agua
carne: bovina
```

## Matriz ou lista

```yaml
frutas:
- laranja
- manga
- banana

legumes:
- cenoura
- couve-flor
- tomate
```

## Dicionários

```yaml
Banana:
  Calorias: 105
  Gorduras: 0,4 g
  Carboidratos: 27 g
Uvas:
  Calorias: 62
  Gorduras: 0,3 g
  Carboidratos: 16 g
```

## Playbook Ansible

Segue um exemplo de playbook Ansible, no arquivo playbook.yml:

```yaml
---
- hosts: webserver
  sudo: yes
  remote_user: ec2-user
  tasks:
  - name: Updating System
    yum:
      name=*
      state=latest
  - name: atualizar teste
    apt:
      name=*
      state=latest
...
```
