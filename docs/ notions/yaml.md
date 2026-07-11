# YAML

YAML est un format de fichier utilisé pour écrire des données structurées de manière lisible. On le rencontre souvent dans les fichiers de configuration.

Dans ce dépôt, YAML est utilisé dans deux fichiers importants :

- `mkdocs.yml`, pour configurer le site ;
- `.gitlab-ci.yml`, pour configurer l'intégration continue GitLab.

## Un format basé sur l'indentation

YAML utilise les espaces pour organiser les informations. Les tabulations sont
à éviter.

Exemple :

```yaml
site_name: Mini site de master

nav:
  - Accueil: index.md
  - Guide:
      - Bien démarrer: guide/demarrage.md
```

Dans cet exemple :

- `site_name` contient une valeur simple ;
- `nav` contient une liste ;
- `Guide` contient une sous-liste.

## Les formes les plus fréquentes

### Clé et valeur

```yaml
language: fr
```

### Liste

```yaml
plugins:
  - search
```

### Liste d'objets

```yaml
palette:
  - scheme: default
    primary: teal
  - scheme: slate
    primary: teal
```

## YAML dans Ansible

Ansible est un outil d'automatisation informatique. Il utilise YAML pour décrire des actions à exécuter sur une ou plusieurs machines.

Un fichier Ansible typique s'appelle un playbook.

```yaml
- name: Installer et démarrer un serveur web
  hosts: serveurs_web
  become: true

  tasks:
    - name: Installer nginx
      ansible.builtin.apt:
        name: nginx
        state: present

    - name: Démarrer nginx
      ansible.builtin.service:
        name: nginx
        state: started
```

Ce fichier décrit des intentions : installer un paquet, démarrer un service,
appliquer une configuration. Ansible lit le YAML et exécute les opérations.

## Pourquoi YAML est utile

YAML est apprécié parce qu'il est :

- lisible par des humains ;
- structuré ;
- adapté aux configurations ;
- facile à versionner avec Git ;
- utilisé par de nombreux outils.

## Sources officielles

- [Spécification officielle YAML 1.2.2](https://yaml.org/spec/1.2.2/)
- [Documentation officielle Ansible - Playbooks](https://docs.ansible.com/projects/ansible/latest/playbook_guide/playbooks_intro.html)
