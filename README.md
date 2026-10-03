# Apache Iceberg: коллекция ссылок и материалов

Куда смотреть, чтобы разобраться в открытом табличном формате Apache Iceberg и его экосистеме: официальные доки, каталоги, движки, облачные сервисы и материалы на русском языке. Подборка ведётся вручную.

Обозначения: ✅ — ссылка проверена; ⚠️ — сайт не даёт проверить автоматически, но ресурс указан в официальных источниках.

## Содержание

- [Русскоязычные материалы](#русскоязычные-материалы)
- [Курсы на английском](#курсы-на-английском)
- [Документация и спецификация](#документация-и-спецификация)
- [Каталоги и REST Catalog](#каталоги-и-rest-catalog)
- [Движки запросов и библиотеки](#движки-запросов-и-библиотеки)
- [Песочницы и демо](#песочницы-и-демо)
- [Производительность и обслуживание](#производительность-и-обслуживание)
- [Time Travel и ветвление](#time-travel-и-ветвление)
- [Облачные платформы](#облачные-платформы)
- [Статьи, книги, видео](#статьи-книги-видео)
- [Сообщества](#сообщества)

## Русскоязычные материалы

- [Полный курс SubQuery](https://subquery.ru/course/iceberg) — 6 глав и 19 уроков с упражнениями, всё на русском.
- [DuckDB и Apache Iceberg](https://subquery.ru/blog/duckdb-iceberg) — лейкхаус без кластера: подключение, ускорение запросов, подводные камни.
- [Пять причин медленных Iceberg-запросов](https://subquery.ru/blog/iceberg-queries-speedup) — как найти и починить структурные проблемы таблиц.
- [Работаем с Iceberg из Trino и DuckDB](https://subquery.ru/blog/iceberg-trino-duckdb) — практика без «большой» СУБД.
- [Лейкхаус как у Google](https://subquery.ru/blog/6-layer-lakehouse-from-google) — разбор шести слоёв производительности Borderless Lakehouse.

## Курсы на английском

- [Apache Iceberg and Tableflow (Tim Berglund)](https://www.timberglund.com/videos/apache-iceberg-course) ✅ — видеокурс одного из создателей формата.
- [Плейлист курса на YouTube](https://www.youtube.com/playlist?list=PLf38f5LhQthcLN84xP6JgQ-pEbAc8SbSi) ⚠️ — те же модули на канале Confluent.

## Документация и спецификация

- [Официальный сайт](https://iceberg.apache.org/) ✅ — обзор возможностей и навигация по проекту.
- [Документация](https://iceberg.apache.org/docs/latest/) ✅ — концепции, конфигурация, интеграции.
- [Спецификация](https://iceberg.apache.org/spec/) ✅ — полное описание формата v1–v3.
- [Релизы](https://iceberg.apache.org/releases/) ✅ — версии и артефакты.
- [Блог проекта](https://iceberg.apache.org/blog/) ✅ — новости и технические заметки.

## Каталоги и REST Catalog

- [Урок про каталоги](https://subquery.ru/blog/courses/iceberg/catalogs) — как выбрать каталог под свои задачи.
- [Спецификация REST Catalog](https://iceberg.apache.org/docs/latest/rest-protocol/) ✅ — протокол, эндпоинты, выдача учётных данных.
- [Настройка REST-клиента](https://iceberg.apache.org/docs/latest/rest-catalog/) ✅ — Spark/Flink, OAuth2 и SigV4.
- [Apache Polaris](https://polaris.apache.org/) ✅ — открытый каталог ASF, поддерживающий REST API Iceberg.
- [Polaris на GitHub](https://github.com/apache/polaris) ✅ — код и quickstart.
- [Lakekeeper](https://lakekeeper.io/) ✅ — быстрый REST-каталог на Rust с контролем доступа.
- [Lakekeeper на GitHub](https://github.com/lakekeeper/lakekeeper) ✅ — исходники и примеры.
- [Project Nessie](https://projectnessie.org/) ✅ — каталог с Git-подобными ветками.
- [AWS Glue](https://iceberg.apache.org/docs/latest/aws/#glue-catalog) ✅ — Glue Catalog в роли каталога Iceberg.
- [Hive Metastore](https://iceberg.apache.org/docs/latest/hive/) ✅ — глобальный каталог поверх Hive.

## Движки запросов и библиотеки

- [Экосистема движков](https://subquery.ru/blog/courses/iceberg/query-engines-and-ecosystem) — обзор Spark, Flink, Trino и Python-инструментов.
- [Обзор Trino](https://subquery.ru/blog/trino) — статья про движок и его интеграции.
- [DuckDB Iceberg extension](https://duckdb.org/docs/current/core_extensions/iceberg/overview.html) ✅ — чтение, запись и ATTACH к REST-каталогу.
- [Trino Iceberg connector](https://trino.io/docs/current/connector/iceberg.html) ✅ — коннектор, метатаблицы, процедуры.
- [Spark Quickstart](https://iceberg.apache.org/spark-quickstart/) ✅ — стартовый стенд со Spark.
- [Flink Quickstart](https://iceberg.apache.org/flink-quickstart/) ✅ — потоковая работа с Flink.
- [PyIceberg](https://py.iceberg.apache.org/) ✅ — Python без JVM, Arrow и Pandas.
- [iceberg-rust](https://github.com/apache/iceberg-rust) ✅ — реализация формата на Rust.
- [ClickHouse: Iceberg engine](https://clickhouse.com/docs/en/engines/table-engines/integrations/iceberg) ✅ — табличный движок в ClickHouse.

## Песочницы и демо

- [Упражнение: каталоги](https://subquery.ru/blog/courses/iceberg/catalogs-exercise) — первая таблица и снапшоты.
- [Упражнение: эволюция схемы](https://subquery.ru/blog/courses/iceberg/schema-evolution-exercise) — правки структуры без переписывания.
- [Упражнение: партицирование](https://subquery.ru/blog/courses/iceberg/partitioning-exercise) — партиции и pruning.
- [Упражнение: time travel](https://subquery.ru/blog/courses/iceberg/timetravel-exercise) — история таблицы на практике.
- [Упражнение: ветвление и теги](https://subquery.ru/blog/courses/iceberg/branching-exercise) — Git-подобный workflow.
- [Упражнение: обслуживание](https://subquery.ru/blog/courses/iceberg/maintenance-exercise) — очистка и оптимизация.
- [docker-spark-iceberg](https://github.com/databricks/docker-spark-iceberg) ✅ — готовый стенд Spark + MinIO.
- [Nessie Sandbox](https://projectnessie.org/guides/try-nessie/) ✅ — Nessie и MinIO в Docker.
- [Примеры Lakekeeper](https://github.com/lakekeeper/lakekeeper/tree/main/examples) ✅ — ноутбуки для знакомства.

## Производительность и обслуживание

- [Партицирование и эволюция](https://subquery.ru/blog/courses/iceberg/partitioning-and-partition-evolution) — hidden partitioning и трансформации.
- [Кластеризация](https://subquery.ru/blog/courses/iceberg/clustering) — Z-ordering и сравнение с партициями.
- [Метатаблицы](https://subquery.ru/blog/courses/iceberg/metadata-tables) — диагностика через SQL.
- [Обслуживание таблиц](https://subquery.ru/blog/courses/iceberg/table-maintenance) — снапшоты, компакция, гигиена.
- [Maintenance (доки)](https://iceberg.apache.org/docs/latest/maintenance/) ✅ — официальный гайд.
- [RisingWave: small files](https://risingwave.com/blog/iceberg-small-file-problem/) ✅ — мелкие файлы и стратегии компакции.
- [Dremio: small files problem](https://www.dremio.com/blog/apache-iceberg-small-files-problem-causes-fixes-and-prevention/) ⚠️ — причины и профилактика.
- [Expire Snapshots / Orphan Files](https://iceberglakehouse.com/iceberg/iceberg-expire-snapshots/) ⚠️ — справочник по очистке.

## Time Travel и ветвление

- [Time travel и откат](https://subquery.ru/blog/courses/iceberg/timetravel-and-rollback) — запросы к старым версиям.
- [Теги и ветки](https://subquery.ru/blog/courses/iceberg/tagging-and-branching) — Write-Audit-Publish.
- [Branching and Tagging (доки)](https://iceberg.apache.org/docs/latest/branching/) ✅ — официальное описание референсов.
- [Time Travel (справочник)](https://iceberglakehouse.com/iceberg/iceberg-time-travel/) ✅ — синтаксис в разных движках.

## Облачные платформы

- [Snowflake](https://docs.snowflake.com/en/user-guide/tables-iceberg) ⚠️ — Iceberg-таблицы в Snowflake.
- [BigQuery](https://cloud.google.com/bigquery/docs/iceberg-tables) ✅ — managed и внешние таблицы.
- [AWS Athena](https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg.html) ✅ — запросы и запись в AWS.
- [Databricks](https://docs.databricks.com/gcp/en/iceberg/) ✅ — Iceberg в Unity Catalog.
- [Borderless Lakehouse](https://cloud.google.com/blog/products/data-analytics/introducing-the-borderless-lakehouse) ✅ — федерация каталогов в BigQuery.

## Статьи, книги, видео

- [Ryan Blue: A High-Performance Format](https://www.dremio.com/blog/iceberg-a-high-performance-format-for-huge-analytic-tables/) ⚠️ — классическая статья создателя Iceberg.
- [Архитектура Iceberg под капотом](https://www.dremio.com/blog/apache-iceberg-an-architectural-look-under-the-covers/) ⚠️ — манифесты, метаданные, снапшоты.
- [Iceberg Knowledge Base](https://iceberglakehouse.com/iceberg/) ✅ — энциклопедия терминов и практик.
- [The Definitive Guide (companion)](https://github.com/developer-advocacy-dremio/definitive-guide-to-apache-iceberg) ✅ — примеры кода к книге O'Reilly.
- [Talks и Iceberg Summit](https://iceberg.apache.org/talks/) ✅ — записи докладов.
- [YouTube @ApacheIceberg](https://www.youtube.com/@ApacheIceberg) ✅ — официальный канал.

## Сообщества

- [apache/iceberg на GitHub](https://github.com/apache/iceberg) ✅ — основной репозиторий.
- [Dev mailing list](https://lists.apache.org/list.html?dev@iceberg.apache.org) ✅ — рассылка разработчиков.
- [Slack-приглашение](https://s.apache.org/iceberg-slack) ✅ — оперативные обсуждения.
- [Telegram: Data Engineers](https://t.me/data_engineers) ⚠️ — русскоязычное сообщество.
- [Telegram: BigData team](https://t.me/bigdata_team) ⚠️ — канал про большие данные.
- [Telegram: DataHub RU](https://t.me/datahub_ru) ⚠️ — обсуждение инструментов.

## Вклад

Если знаете хороший ресурс — откройте issue или pull request. Ссылка должна быть рабочей и относиться к Apache Iceberg.