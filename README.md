![Grafo de Fluxo](https://github.com/user-attachments/assets/e2a1a1e4-9345-424a-91f5-0748d80156cc)

Complexidade Ciclomática:

M=E−N+2 P
Cálculo :
M=8−6+2×1=4
complexidade ciclomática é 4 .

Caminhos básicos:

Caminho 1 : 1 → 2 (Conexão bem-sucedida) → 3 → 4 (Executa a consulta) → 5 → 5b (Consulta não retorna resultado) → 6 (Retorna false).

Caminho 2 : 1 → 2 (Conexão bem-sucedida) → 3 → 4 (Executa a consulta) → 5 → 5a (Consulta retorna resultado) → 6 (Retorna true).

Caminho 3 : 1 → 2 (Falha ao conectar ao banco de dados, executa o bloco catch) → 6 (Retorna false).

Caminho 4 : 1 → 2 → 3 (Conexão bem-sucedida, mas uma falha na execução do SQL leva ao bloco catch) → 6 (Retorna false).
