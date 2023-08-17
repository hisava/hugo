---
title: "debian"
date: 2023-08-17T09:59:38+03:00
draft: false
---

# Установка debian

на virtualbox ( windows )

## 1

[Выбираем версию](https://download.virtualbox.org/virtualbox) virtualbox для windows

Например, [VirtualBox 7.0.10](https://download.virtualbox.org/virtualbox/7.0.10/VirtualBox-7.0.10-158379-Win.exe)

`VirtualBox-7.0.10-158379-Win.exe`

Скачиваем и устанавливаем 

## 2

Не забываем так же установить [дополнения для virtualbox](https://download.virtualbox.org/virtualbox/7.0.10/Oracle_VM_VirtualBox_Extension_Pack-7.0.10.vbox-extpack)

`Oracle_VM_VirtualBox_Extension_Pack-7.0.10.vbox-extpack`

( Клавиша `CTRL+T` в virtualbox открывает менеджер плагинов )

## 3

[Выбираем версию](https://cdimage.debian.org/debian-cd) debian

Например, [debian 12.1.0](https://cdimage.debian.org/debian-cd/12.1.0/amd64/bt-cd) или [сразу скачать torrent](https://cdimage.debian.org/debian-cd/12.1.0/amd64/bt-cd/debian-12.1.0-amd64-netinst.iso.torrent)

## 4

Запускаем virtualbox и создаём машину `CTRL+N`

+ Имя: deb

+ Образ ISO: debian-12.1.0-amd64-netinst.iso

+ Пропустить автоматическую установку

+ Готово

## 5

Запустить 

## 6

Graphical install

## 7

English - Continue

Unated States - Continue 

American English - Continue  

## 8

Hostname - ex - Continue 

Domain - Continue

Root password - 12 - Continue 

Full name - Continue 

Username - al - Continue 

password - 12 - Continue 

Eastern - Continue 

## 9

Guided - use entire disk - Continue - Continue

All files in one partition - Continue

Finish partitioning and write changes to disk - Continue

Yes - Continue

## 10

Scan extra installation media ? - Continue - Continue 

deb.debian.org - Continue - Continue

## 11

Select and install software

Participate ? - Continue 

+ [x] Debian desktop environment

+ [x] ... MATE

+ [x] ... standard system utilites

Continue

## 12

Всё
