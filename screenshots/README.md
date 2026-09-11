# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
* Travis CI showing a successful build and deploy job

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```


Travis CI Note
Travis CI was successfully connected to the repository, and a build execution was triggered.

However, it was not possible to obtain a successful build due to Travis CI account plan/credit limitations. As shown in the attached screenshot, Travis CI rejected the build request because the account is not enrolled in a supported pricing plan.

Because of this limitation, no active webhook or complete pipeline execution could be generated.

All other project requirements, including Docker image publication, AWS infrastructure provisioning, Kubernetes deployment, services, HPA configuration, and logging verification, were completed successfully.


O Travis CI foi conectado com sucesso ao repositório e uma execução do pipeline foi iniciada.

Entretanto, não foi possível obter um build bem-sucedido devido às limitações de créditos/plano da conta Travis CI. Conforme demonstrado na captura de tela anexada, o Travis CI rejeitou a execução porque a conta não está vinculada a um plano compatível.

Devido a essa limitação, não foi possível gerar um webhook ativo nem concluir a execução completa do pipeline.

Todos os demais requisitos do projeto, incluindo publicação das imagens Docker, provisionamento da infraestrutura AWS, implantação no Kubernetes, configuração de