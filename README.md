# Домашнее задание к занятию «Установка Kubernetes» Стасенко Григорий Михайлович

### Цель задания

Установить кластер K8s.

### Чеклист готовности к домашнему заданию

1. Развёрнутые ВМ с ОС Ubuntu 20.04-lts.


### Инструменты и дополнительные материалы, которые пригодятся для выполнения задания

1. [Инструкция по установке kubeadm](https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm/).
2. [Документация kubespray](https://kubespray.io/).

-----

### Задание 1. Установить кластер k8s с 1 master node

1. Подготовка работы кластера из 5 нод: 1 мастер и 4 рабочие ноды.
2. В качестве CRI — containerd.
3. Запуск etcd производить на мастере.
4. Способ установки выбрать самостоятельно.

## Решение

С помощью terraform развернули 5 машин с заданными характеристиками:

<img width="1019" height="289" alt="image" src="https://github.com/user-attachments/assets/54e49702-2eb2-45df-96a6-78286984c15e" />

На них  развернули K8s, подключили друг к другу.
CNI-плагин использован Flannel.

<img width="620" height="170" alt="image" src="https://github.com/user-attachments/assets/025cd098-42f9-49c7-bf66-3b13590525df" />
