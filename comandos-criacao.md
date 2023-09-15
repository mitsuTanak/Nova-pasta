# Comando SQL - Referencia
<!----------------------------------------------------------->

## Modelagem fisica

### Criar banco de dados
```sql
CREATE DATABASE vendas CHARACTER SET utf8mb4;

``` 

<!-- ------------------ -->

```sql
CREATE TABLE fabricantes(
    id INT NOT NULL Primary KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL
)
```

<!--  -->

```sql
CREATE TABLE produtos(
    id INT NOT NULL Primary KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL
    descricao TEXT(1000) NOT NULL,
    quantidade TINYINT(4) NOT NULL
)
```