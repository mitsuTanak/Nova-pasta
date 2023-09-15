# Comando SQL - Referencia
<!-- _____________________________________________________ -->

## Modelagem fisica

### Criar banco de dados
```sql
CREATE DATABASE vendas CHARACTER SET utf8mb4;

``` 

<!-- _____________________________________________________ -->

<!-- h3 -->
### Criar Tabela de Fabricante
```sql
CREATE TABLE fabricantes(
    id INT NOT NULL Primary KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL
)
```

<!--_____________________________________________________ -->

<!-- h3 -->
### Criar Tabela de Produtos

```sql
CREATE TABLE produtos(
    id INT NOT NULL Primary KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL,
    descricao TEXT(1000) NOT NULL,
    preco DECIMAL (6,2) NOT NULL,
    quantidade TINYINT(4) NOT NULL
)
```

<!-- _____________________________________________________ -->

<!-- h3 -->
### Adicionar Campo/Coluna em uma Tabela

```sql
ALTER TABLE produtos ADD fabricante_id INT NOT NULL
AFTER quantidade
```

<!-- _____________________________________________________ -->
### Criação de chave estrangeira (relacionamento entre tabelas)

<!-- h3 -->
```sql
ALTER TABLE produtos

# "CONSTRAINT" é uma restrição definida no relacionamento
ADD CONSTRAINT fk_fabricantes

# A chave estrangeira de fazer referencia a chave primaria
FOREIGN KEY(fabricante_id) REFERENCES fabricantes(id)
```


<!-- _____________________________________________________ -->
###

<!--  -->