# E-commerce de Venda de Livros 

<p>Esta pasta contém o projeto de e-commerce dedicado à venda de livros e artigos relacionados ao universo da leitura. O objetivo é desenvolver o DER - Diagrama de entidade Relacional.</p>

## Mini-mundo

<p>Imagine a seguinte situação em um clube do livro Queremos coletar os dados pessoais de nossos clientes, como se ele é pessoa física ou jurídica. No caso de PF o seu CPF e RG, e no caso de jurídica o CNPJ e IE. Além disso, queremos coletar e armazenar o seu nome, endereço, telefone e e-mail.</p>
<p>O produto principal do e-commerce são livros. Estes livros têm informações associadas a eles como o título, categoria, o ISBN (International Standard Book Number), o ano de publicação, o valor, a editora que publicou o livro, bem como o autor ou autora da obra.</p>
<p>Os livros são fornecidos por editoras. Precisamos ter guardados o telefone da editora, o nome de contato, o e-mail e no máximo 2 telefones.</p>
<p>Sabemos que não podemos ter o mesmo livro vindo de várias editoras. O livro é exclusivo de uma editora.</p>
<p>Nosso cliente pode comprar um ou mais livros através de um pedido de compra. Porém, sempre que ele faz uma compra precisamos verificar no estoque se o livro está ou não disponível antes de efetuar a operação.</p>

## Entidades

- **Cliente**: Armazena informações básicas dos clientes.
- **Livro**: Armazena informações básicas sobre os livros.
- **Editora**: Armazena informações sobre a editora dos livros. 
- **Pedido de Compra**: 
- **Estoque**: Armazenas imformações sobre o estoque do cliente.

## Entidades e Relacionamentos

- **Cliente** – Faz – **Pedido**
- **Pedido** – Contém – **Livro**
- **Livro** – Pertence – **Editora**
- **Estoque** – Existe – **Livro**

## Entidades e Atributos

- **Cliente**: 
  - Tipo: física ou jurídica
  - Atributos:
    - CPF e RG (para pessoas físicas)
    - CNPJ e IE (para pessoas jurídicas)
    - Nome
    - Endereço
    - Telefone
    - E-mail

- **Livro**: 
  - Atributos:
    - Título
    - Categoria
    - ISBN
    - Ano de publicação
    - Preço
    - Editora (referência à editora que publica o livro)

- **Editora**: 
  - Atributos:
    - Nome
    - Telefone de contato
    - E-mail
    - Até dois números de telefone

- **Pedido de Compra**: 
  - Atributos:
    - Data do pedido
    - Status (ex: pendente, concluído)
    - Total

- **Estoque**: 
  - Atributos:
    - Livro (referência ao livro)
    - Quantidade disponível

<p>Este projeto visa não apenas a implementação de um sistema de e-commerce, mas também a aplicação prática de conceitos de modelagem de dados. Espera-se que as informações armazenadas ajudem a otimizar o processo de vendas e a gestão do estoque.</p>
