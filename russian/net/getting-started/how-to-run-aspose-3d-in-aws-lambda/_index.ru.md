---
title: Как запустить Aspose.3D в AWS Lambda
type: docs
description: Интегрируйте функциональность Aspose.3D в свое приложение с помощью Docker независимо от того, какая технология находится в вашем стеке разработки. Узнайте, как использовать Aspose.3D в контейнере Docker
weight: 141
url: /ru/net/how-to-run-aspose-3d-in-aws-lambda/
---
## Подготовка среды AWS

1. Зарегистрировать аккаунт AWS:
[Зарегистрировать аккаунт AWS](https://aws.amazon.com/)
1. Войдите в свою учетную запись AWS, добавьте пользователя IAM под своей учетной записью. Вы можете обратиться к официальному документу AWS:
[Добавить пользователя IAM](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started_create-admin-group.html)
1. Добавьте разрешение «AmazonS3FullAccess», используйте тот же способ, добавьте EC2 и эластичный бобовый стебель, полный доступ для каждого.
1. На последнем шаге убедитесь, что вы получили имя пользователя IAM, ключ, идентификатор ключа и файл «credentials.csv», вам нужно хорошо их сохранить.
Теперь убедитесь, что у вашего пользователя IAM есть S3, EC2, Elastic Beanstalk, полный доступ. См.:
   
**! [AWS Access(AwsAccess.png)**

## Установка набора инструментов AWS для Visual Studio

1. Установите Visual Studio 2019 или более позднюю версию.
1. Загрузите и установите AWS Toolkit для Visual Studio:
[AWS Инструментарий](https://aws.amazon.com/visualstudio/)

## Создать проект, работающий в AWS Lambda

1. Создайте базовое веб-приложение ASP .NET в Visual Studio, напишите тестовый код и получите Aspose.3D с nuget.

1. Убедитесь, что тестовый проект хорошо работает на локальной машине, а затем разверните его в AWS Elastic Beanstalk:
Щелкните правой кнопкой мыши название проекта, выберите "Опубликовать в AWS Elastic Beanstalk". (Эта опция будет существовать только после установки AWS Toolkit for Visual Studio).
1. Вам нужно будет добавить нового пользователя с вашей учетной записью AWS и пользователем IAM, вы можете импортировать файл "credentials.csv", который вы получите на предыдущем шаге.
1. Опубликовать успех, вы получите адрес ссылки, например: `http://testprojectaspose-test.us-west-2.elasticbeanstalk.com/`
Подождите 10 минут, пока ссылка вступит в силу, и вы сможете посетить ее!
