# Задание 1. Модульная инфраструктура для нескольких сред

### `main.tf`
- Создаётся схема виртуальной машины и сети
- Используются **только переменные** – никаких значений напрямую

### `variables.tf`
- Описываются типы и **значения по умолчанию** для переменных

### `terraform.tfvars`
- Содержит значения переменных (токены, пути, количество ядер, RAM, размер диска и т.д.)
- Индивидуальная конфигурация для **каждого окружения**:
  - `Task1Advanced/envs/dev/terraform.tfvars`
  - `Task1Advanced/envs/prod/terraform.tfvars`
  - `Task1Advanced/envs/stage/terraform.tfvars`

## Инициализация каталога

```bash
cd Task1Advanced/modules/vm
terraform init
```

## Запуск

- Используются **разные конфигурации** для окружений `dev`, `stage`, `prod`
- Основная разница – в характеристиках виртуальой машины: **количество ядер, RAM и размер диска**
- Параметры`terraform.tfvars` :

| Переменная   | Описание                                                                 |
|--------------|--------------------------------------------------------------------------|
| `token`      | [OAuth-токен](https://oauth.yandex.ru/verification_code)                 |
| `cloud_id`   | Идентификатор облака в Yandex Cloud                                      |
| `folder_id`  | Идентификатор каталога в Yandex Cloud                                    |

*Оригинальные файлы не добавлены в git для конфиденциальности, но можно воспользоваться примерами для заполнения для каждого окружения*

Для применения конфигурации конкретного окружения `dev`:

```
terraform apply -var-file="../../envs/dev/terraform.tfvars"
```

## Вывод

![result_1.png](https://github.com/kuznechek/architecture-pro-future_2_0/blob/feature/TaskAdvanced1/src/result_1.png)
