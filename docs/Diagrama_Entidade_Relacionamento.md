

DIAGRAMA ENTIDADE RELACIONAMENTO DO APP CONTROLE DE ESTOQUE PARA ABRIGOS



+----------------+      +-----------------+      +------------------+
|     Usuário    |      |     Gerencia    |      |     Abrigo       |
|----------------|      |-----------------|      |------------------|
| PK | ID        | 1  n | FK | UserID     | n  1 | PK | AbrigoID    |
|    | Nome      |------| FK | AbrigoID   |------|    | Nome        |
|    | Email     |      +-----------------+      |    | Localização |
|    | Senha     |                               +------------------+
|    | Tipo      |
+----------------+

+----------------+      +----------------+       +-----------------+
|    Categoria   |      |     Item       |       |    Doação       |
|----------------|      |----------------|       |-----------------|
| PK | ID        | 1  n | PK | ItemID    | n  1  | PK | DoacaoID   |
|    | Nome      |------|    | Nome      |------ | FK | ItemID     |
+----------------+      |    | Quantidade|       |    | Quantidade |
                        | FK | CategoryID|       |    | Data       |
                        | FK | AbrigoID  |       |    | Doador     |
                        +----------------+       | FK | AbrigoID   |
                                                 +-----------------+
