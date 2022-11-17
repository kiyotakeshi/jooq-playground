# jooq-playground

```shell
docker compose up -d
```

```sql
CREATE TABLE `author`
(
    `id`         int NOT NULL,
    `first_name` varchar(255) DEFAULT NULL,
    `last_name`  varchar(255) DEFAULT NULL,
    PRIMARY KEY (`id`)
);

INSERT INTO sample.author (id, first_name, last_name)
VALUES (1, 'mike', 'popcorn'),
       (2, 'kendrick', 'west');
```

```shell
$ java -version                      
openjdk version "17.0.3.1" 2022-04-22 LTS

$ mvn --version                                                          
Apache Maven 3.8.6 (84538c9988a25aec085021c365c560670ad80f63)

mvn clean install
# mvn clean jooq-codegen:generate
```

run [main class](./src/main/java/org/example/jooqPlayground/Main.java) using IDE 
