# Домашнее задание к занятию 2. «Применение принципов IaaC в работе с виртуальными машинами» - Розаев А.Ю.

#### Это задание для самостоятельной отработки навыков и не предполагает обратной связи от преподавателя. Его выполнение не влияет на завершение модуля. Но мы рекомендуем его выполнить, чтобы закрепить полученные знания. Все вопросы, возникающие в процессе выполнения заданий, пишите в раздел "Вопросы по заданиям" в личном кабинете.
---
## Важно

**Перед началом работы над заданием изучите [Инструкцию по экономии облачных ресурсов](https://github.com/netology-code/devops-materials/blob/master/cloudwork.MD).**
Перед отправкой работы на проверку удаляйте неиспользуемые ресурсы.
Это нужно, чтобы не расходовать средства, полученные в результате использования промокода.
Подробные рекомендации [здесь](https://github.com/netology-code/virt-homeworks/blob/virt-11/r/README.md).

---

### Цели задания

1. Научиться создвать виртуальные машины в Virtualbox с помощью Vagrant.
2. Научиться базовому использованию packer в yandex cloud.

---

## Задача 1

На ВМ установлены VirtualBox, Vagrant, Packer + плагин от Яндекс Облако, уandex cloud cli:

![VM](https://github.com/expgt/net-fops-hw-14-2/blob/main/14_2_1.png)

---

## Задача 2

Создана ВМ Virtualbox с помощью Vagrant с установленым Docker:

![VM_Virtualbox](https://github.com/expgt/net-fops-hw-14-2/blob/main/14_2_2.png)

---

## Задача 3

- Создан образ с помощью Packer, в образ добавлены Docker, Htop и Tmux

![Image](https://github.com/expgt/net-fops-hw-14-2/blob/main/14_2_3.png)

- Создана новая ВМ в облаке, использован данный образ

![VM_YC](https://github.com/expgt/net-fops-hw-14-2/blob/main/14_2_4.png)

- Произведено подключение по ssh и проверена установка Docker, Htop и Tmux

![SSH](https://github.com/expgt/net-fops-hw-14-2/blob/main/14_2_5.png)

- Файл для создания образа

[Packer_file](https://github.com/expgt/net-fops-hw-14-2/blob/main/mydebian.json)

