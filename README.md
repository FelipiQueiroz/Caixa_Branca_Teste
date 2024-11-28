![Grafo de Fluxo](https://github.com/user-attachments/assets/00247d2c-621d-4f41-ae5a-a14b20c0eabe)
![grafo de fluxo](https://github.com/user-attachments/assets/a3fc46a8-0c82-47cf-822b-7623f81748a4)

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
