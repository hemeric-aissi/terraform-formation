# Formation Terraform

Ce dépôt rassemble mes notes et exercices de formation sur [Terraform](https://developer.hashicorp.com/terraform/docs).

## Premiers pas

Dans Git Bash, vérifier l'installation :

```bash
terraform version
```

Commandes courantes, à exécuter dans un dossier contenant une configuration Terraform :

```bash
terraform init      # Initialise le dossier de travail
terraform fmt       # Formate les fichiers de configuration
terraform validate  # Vérifie la configuration
terraform plan      # Prévisualise les changements
terraform apply     # Applique les changements après confirmation
terraform destroy   # Détruit les ressources gérées après confirmation
```

Les commandes `apply` et `destroy` modifient une infrastructure réelle et peuvent entraîner des coûts ou supprimer des ressources.

## Notes

- **Infrastructure as Code (IaC)** : description de l'infrastructure dans des fichiers versionnables.
- **Provider** : extension qui permet à Terraform de communiquer avec une plateforme ou un service.
- **State** : état des ressources gérées par Terraform ; il peut contenir des données sensibles et ne doit pas être publié.

Ne pas enregistrer d'identifiants, de secrets ou de fichiers d'état dans le dépôt. Consulter la [documentation officielle](https://developer.hashicorp.com/terraform/docs) pour approfondir.
