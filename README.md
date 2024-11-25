![Grafo de Fluxo](https://github.com/user-attachments/assets/00247d2c-621d-4f41-ae5a-a14b20c0eabe)

Complexidade Ciclomática:

M=E−N+2 P
Cálculo :
M = 6 - 6 + 2 × 1
M = 2
complexidade ciclomática é 2 .

Caminhos básicos:

Caminho 1:
Início → conectarBD() → Construção SQL → Executar consulta → Decisão rs.next()(true) → Retorno resultado.

Caminho 2:
Início → conectarBD() → Construção SQL → Executar consulta → Decisão rs.next()(false) → Retorno resultado.
