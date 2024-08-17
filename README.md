# Sistema de Gerenciamento de Vendas e Inventário

## Objetivo

O objetivo deste projeto é desenvolver um sistema robusto e eficiente de gerenciamento de inventário para uma loja virtual. O sistema permite o cadastro, atualização, exclusão e listagem de produtos, além de realizar vendas e gerar relatórios detalhados em formato TXT. Foi projetado para lidar com erros de forma elegante e para oferecer uma interface amigável para os usuários.

## Funcionalidades

### 1. Cadastro de Produtos
- **Informações do Produto**: Nome, categoria, preço, quantidade em estoque e descrição opcional.
- **Armazenamento**: Produtos são armazenados utilizando dicionários indexados por um identificador único.

### 2. Atualização de Produtos
- **Atualizações Possíveis**: Preço, quantidade em estoque e descrição.
- **Validação**: Mecanismos de validação para evitar erros comuns, como preços negativos ou estoque insuficiente.

### 3. Exclusão de Produtos
- **Remoção Segura**: Exclusão de produtos do inventário com tratamento de exceções para produtos inexistentes.

### 4. Realização de Vendas
- **Compra de Múltiplos Produtos**: Clientes podem comprar múltiplos produtos em quantidades variáveis.
- **Atualização de Estoque**: Estoque atualizado automaticamente após cada venda.
- **Tratamento de Exceções**: Verificação de estoque insuficiente com mensagens de erro claras.

### 5. Relatórios de Vendas
- **Formato CSV**: Geração de relatórios em formato CSV contendo informações detalhadas da venda.
- **Informações Incluídas**: Nome do produto, quantidade vendida, preço unitário, valor total da venda e data/hora da transação.

### 6. Persistência de Dados
- **Arquivos de Dados**: Dados do inventário e informações de vendas são persistidos em arquivos de texto ou CSV, garantindo a persistência entre execuções.
- **Manipulação de Arquivos**: Utiliza o módulo `csv` do Python para manipulação segura dos arquivos de dados.

### 7. Tratamento de Exceções
- **Exceções Personalizadas**: Tratamento robusto de exceções para cadastro, atualização, exclusão e manipulação de dados.
- **Erros de Estoque**: Exceções personalizadas para erros de estoque insuficiente e manipulação inadequada de dados.

### 8. Interface com o Usuário
- **Interação Amigável**: Menus e opções claras que guiam o usuário durante o uso do sistema.
- **Flexibilidade**: Uso de funções com parâmetros variáveis (*args, **kwargs) para maior flexibilidade.

### 9. Técnicas Funcionais
- **Programação Funcional**: Uso de `map`, `filter`, `reduce` e funções lambda para manipulação e processamento eficiente de listas de produtos e vendas.

### 10. Documentação
- **Documentação Completa**: Descrição detalhada da arquitetura, decisões de design e exemplos de uso para facilitar o entendimento dos usuários.

## Estrutura do Projeto

```plaintext
├── data/
│   ├── estoque_de_produtos.txt
│   └── Relatório_de_vendas.txt
├── src/
│   ├── system.py
├── venv/
├── README.md
└── requirements.txt
