# Automação de Cadastro de Produtos

Projeto desenvolvido em **Python** com o objetivo de automatizar o processo de leitura de uma base de dados e o cadastro desses produtos em um sistema web ou interno. Esta ferramenta é ideal para eliminar tarefas repetitivas e aumentar a produtividade.

---

## Objetivo
O script realiza a leitura de uma base de dados (planilha) e preenche automaticamente os campos do sistema, como: 
* Código do Produto, Marca, Tipo, Categoria, Preços e Observações.

---

## Tecnologias Utilizadas
* **Python**
* **Pandas** (Manipulação de dados)
* **PyAutoGUI** (Automação de interface)
* **Openpyxl** (Suporte para arquivos Excel)

---

## Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/gabgrisolia/automacao-cadastro-produtos.git](https://github.com/gabgrisolia/automacao-cadastro-produtos.git)
    cd automacao-cadastro-produtos
    ```

2.  **Instale as bibliotecas necessárias:**
    Você precisará do Pandas, PyAutoGUI e Openpyxl. Instale todos de uma vez com o comando:
    ```bash
    pip install pyautogui pandas openpyxl
    ```

3.  **Prepare a base de dados:**
    Certifique-se de que o arquivo de dados (ex: `produtos.csv`) esteja na mesma pasta do script Python.

4.  **Execute o script:**
    ```bash
    python codigo.py
    ```

---

## Funcionamento do Script
1.  **Acesso:** O script abre o navegador e faz login no sistema.
2.  **Leitura:** O **Pandas** extrai as informações da planilha.
3.  **Automação:** O **PyAutoGUI** assume o controle do mouse/teclado para preencher os campos.
4.  **Repetição:** O processo se repete automaticamente para cada linha da base de dados.

---

## Segurança (Fail-Safe)
* **Interrupção:** Para parar o script imediatamente, mova o mouse para qualquer **canto da tela**.
* **Pausa:** O código utiliza `pyautogui.PAUSE` para garantir que o sistema acompanhe a velocidade da digitação.

---

## 👤 Autor
Desenvolvido por **Gabriela Grisolia**.
* GitHub: [gabgrisolia](https://github.com/gabgrisolia)