docker build --tag=k8s-play .
docker run -it --rm --name k8s-play k8s-play

docker run -v C:\Users\user\.kube:/kube -v C:\Users\user\.aws:/root/.aws/ --env KUBECONFIG=/kube/config -it --rm k8s-play
