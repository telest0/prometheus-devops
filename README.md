# Kubectl OpenAI plugin ✨

This project is a `kubectl` plugin to generate and apply Kubernetes manifests using OpenAI GPT.

- Generate Open AI API key
- Install kubectl OpenAI plugin
- Set environment variable `export OPENAI_API_KEY=<your OpenAI key>`
- Make a request like kubectl as in the table below

## Prompt portfolio

|    Name    |     Prompt     |   Description |      Example       |
|------------|----------------|---------------|--------------------|
| app.yaml | create app pod | Create an application in pod | [app.yaml](./yaml/app.yaml) |
| app-configmap.yaml     | create redis pod with configmap | Store non-confidential data in key-value pairs | [app-configmap.yaml](./yaml/app-configmap.yaml) |
| app-livenessProbe.yaml | create nginx pod and add liveness probe | Liveness probe restarts a cotainer |  [app-livenessProbe.yaml](./yaml/app-livenessProbe.yaml)|
| app-readinessProbe.yaml | create nginx pod and add readiness probe | Readiness probe put a cotainer out of Service LoadBalancer |  [app-readinessProbe.yaml](./yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml  | add volume to a pod | Mounts a file or directory from the host node's filesystem into your Pod |  [app-volumeMounts.yaml](./yaml/app-volumeMounts.yaml)|
| app-cronjob.yaml       | Hello world cronjob | Creates Jobs on a repeating schedule | [app-cronjob.yaml](./yaml/app-cronjob.yaml) | 
| app-job.yaml           | a job that rsync with gsutil from data-input volume | Short time running process in a pod | [app-job.yaml](./yaml/app-job.yaml) |
| app-multicontainer.yaml| a job that rsync with gsutil from data-input volume| Containers that need to work together | [app-multicontainer.yaml](./yaml/app-multicontainer.yaml) |
| app-resources.yaml     | pod with resources limit cpu, mem | how much of each resource a container needs | [app-resources.yaml](./yaml/app-resources.yaml) |
| app-secret-env.yaml    | pod with secret username and password| Attach sensitive data in a pod | [app-secret-env.yaml](./yaml/app-secret-env.yaml) |