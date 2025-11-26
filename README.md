# 🚀 Nginx Load Balancer Visualizer

Simulação visual de um Proxy Reverso (Nginx) distribuindo carga entre duas APIs.

### 📋 Pré-requisitos
* **Docker** e **Docker Compose** instalados.
* **k6** instalado (para o teste de carga).

### ▶️ Como Rodar

1.  **Inicie os serviços:**
    ```bash
    docker-compose up --build
    ```

2.  **Acesse o Dashboard:**
    Abra o navegador em: [http://localhost](http://localhost)
    *(Você verá o gráfico atualizando lentamente)*

3.  **Execute o Teste de Carga (Em outro terminal):**
    ```bash
    k6 run load-test.js
    ```
    *(O gráfico começará a se mover rapidamente, dividindo a carga 50/50)*

4.  **Parar a aplicação:**
    Pressione `Ctrl + C` e execute:
    ```bash
    docker-compose down
    ```
