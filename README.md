# Trading Card Game API REST

(1,2) Este proyecto trata sobre la implementación de una __API REST segura__ donde se compran y venden cartas del juego 
de cartas de Pokemon:
__Trading Card Game (TCG)__.
Estas son las tablas que contendrá:

1. Usuarios
2. Cartas
3. Transacciones

(3) Y estas tablas contendrán los siguientes campos:

1. __Usuarios__:
   - `id` (Long): Identificador único del usuario.
   - `username`(String): Nombre del usuario (único) 
   - `password` (String): Contraseña del usuario (hasheada)
   - `rol` (String): Rol del usuario, puede ser `USER` o `ADMIN`

2. __Cartas__:
    - `id` (Long): Identificador único de la carta en concreto.
    - `nombre`(String): Nombre de la carta (único).
    - `tipo`(String): Tipo de la carta.
    - `vida`(int): Puntos de vida de la carta.
    - `daño`(int): Puntos de daño de la carta.
    - `vendedores` (List<Usuario>): Lista de usuarios que venden la carta.

3. __Transacciones__:
    - `id` (Long): Identificador único de la transacción.
    - `precio` (double): Precio de la transacción.
    - `id_vendedor`(Long): Identificador único del usuario vendedor.
    - `id_comprador`(Long): Identificador único del usuario comprador.
    - `id_carta`(Long): Identificador único de la carta.




