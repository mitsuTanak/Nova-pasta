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
INSERT INTO fabricantes (nome)
VALUE ('Positivo'), ('Microsft')
```

<!-- _____________________________________________________ -->

## Insert
## Produtos

```sql

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id)
VALUE ('Ultrabook', 
'Ultrabook Asus Intel Core i9',
6500.99,
7,
1 --Asus
);

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id)
VALUE ('Geladeira',
'Frost-free com acesso a internet',
8500.99,
10,
6 --Brastemp
);

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id)
VALUE ('Tablet',
'Tablet com 10 polegadas com 256GB de armazenamento',
4999.00,
3,
5 --Sansung
);

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id)
VALUE ('Iphone 14 Pro Max',
'Processador Bionic 15 com 256GB de armazenamento',
9999.95,
7,
3 --Apple
);

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id)
VALUE ('Ipad mini',
'Tablet com tela de oled 4k com 512GB de armazenamento',
6500.99,
7,
3
);
INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id)
VALUE ('XBox Serie X',
'Console de Ultima geração',
4500.00,
6,
8
);
INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id)
VALUE ('Ultrabook',
'Tablet com tela de oled 4k com 512GB de armazenamento',
4500.00,
12,
7
);
```