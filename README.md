# Домашнее задание к занятию «Запуск приложений в K8S»

### Цель задания

В тестовой среде для работы с Kubernetes необходимо развернуть Deployment с приложением, состоящим из нескольких контейнеров, и масштабировать его.

### Чеклист готовности к домашнему заданию

1. Установленное k8s-решение (например, MicroK8S).
2. Установленный локальный kubectl.
3. Редактор YAML-файлов с подключённым git-репозиторием.

### Инструменты и дополнительные материалы

1. [Описание](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/) Deployment и примеры манифестов.
2. [Описание](https://kubernetes.io/docs/concepts/workloads/pods/init-containers/) Init-контейнеров.
3. [Описание](https://github.com/wbitt/Network-MultiTool) Multitool.

## Задание 1. Создать Deployment и обеспечить доступ к репликам приложения из другого Pod

1. Создан Deployment с двумя контейнерами (nginx и multitool):
```bash
kubectl apply -f task1/deployment.yaml
# 3-launchingK8S
