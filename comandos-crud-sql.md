<!--  -->

<!-- h1 -->
# Comandos SQL - Para CRUD Referencia

<!-- h2 -->
## Resumo

C -> Create (insere dados)
R -> Read (ler dados)
U -> Update (atualizar dados)
D -> Delete (excluir dados)

<!-- _____________________________________________________ -->

## Insert
## Fabricantes

```sql

INSERT INTO fabricantes (nome) VALUE ('Asus')
INSERT INTO fabricantes (nome) VALUE ('Dell')
INSERT INTO fabricantes (nome)
VALUE ('Apple'), ('LG'), ('Sansung'), ('Brastemp')
```

<!-- _____________________________________________________ -->

## Insert
## Produtos

```sql

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante)
VALUE ('Ultrabook', 'Ultrabook Asus Intel Core i9')
```