# Technology Radar

Радар оценивает технологии по четырём категориям: **Adopt** (рекомендуется), **Trial** (попробовать), **Assess** (оценить), **Hold** (не использовать).

| Технология | Категория | Пояснение |
|------------|-----------|------------|
| Apache Kafka | Adopt | Основная шина событий, основа асинхронного взаимодействия доменов |
| Apache Iceberg + S3 | Adopt | Data Lakehouse: ACID, time travel, работа с большими данными на S3 |
| Terraform | Adopt | Управление инфраструктурой как кодом (уже внедрён) |
| Kubernetes | Adopt | Оркестрация микросервисов и потоковых приложений |
| Debezium | Trial | CDC из legacy SQL Server 2008 в Kafka |
| Apache Flink / Kafka Streams | Trial | Потоковая обработка, замена batch ETL |
| DataHub / OpenMetadata | Trial | Каталог данных, управление метаданными, data lineage |
| dbt | Trial | Трансформация данных в Lakehouse |
| Power BI / Superset | Assess | BI для Self-Service (окончательный выбор не сделан) |
| GraphQL | Assess | Альтернатива REST для API Gateway |
| Apache Camel | Hold | Устаревшая шина, подлежит замене (Strangler pattern) |
| PowerBuilder | Hold | Легаси, вывод из эксплуатации |
| SQL Server 2008 | Hold | Только как источник CDC для исторических данных, не для новых разработок |
