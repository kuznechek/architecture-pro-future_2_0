# Задание 2. 

1. **Создать бакет Object Storage** в Yandex Cloud для хранения `.tfstate`

2. **Создать сервисный аккаунт** с правами `editor`

3. **В каждой папке окружения (dev/stage/prod) добавить файл [backend.tf](https://github.com/kuznechek/architecture-pro-future_2_0/blob/feature/TaskAdvanced2/envs/dev/backend.tf)** с настройкой бэкенда (endpoint, bucket, key)

4. **Убрать из `main.tf` и `terraform.tfvars` токены и ключи** (они будут передаваться через переменные окружения)

5. **Создать [terraform.yml](https://github.com/kuznechek/architecture-pro-future_2_0/blob/feature/.github/workflows/terraform.yml)**

6. **Добавить секреты в GitHub Actions**:

![terraform.yml](https://github.com/kuznechek/architecture-pro-future_2_0/blob/feature/TaskAdvanced2/src/result_2.png)

7. **Закоммитить код в ветку `feature/task2`**

8. **Запустить apply**