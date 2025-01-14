# cem-helm-charts


Mettre à jour la version du chart : Ouvrez le fichier Chart.yaml et mettez à jour la version du chart. Par exemple, si la version actuelle est 1.0.0, vous pouvez la changer en 1.0.1.

# filepath: /path/to/chart/Chart.yaml
apiVersion: v2
name: my-chart
version: 1.0.1

Empaqueter le chart : Utilisez la commande helm package pour empaqueter le chart avec la nouvelle version.

helm package /path/to/chart

Cette commande créera un fichier .tgz avec le nom et la version du chart, par exemple my-chart-1.0.1.tgz.

Optionnel : Pousser le chart vers un dépôt Helm : Si vous utilisez un dépôt Helm pour stocker vos charts, vous pouvez pousser le nouveau chart vers le dépôt.

helm repo index .
helm push my-chart-1.0.1.tgz my-repo

Assurez-vous que my-repo est correctement configuré dans votre configuration Helm.