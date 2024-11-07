# Loja de Calçados "Passo a Passo" :high_heel:

<p>Esta pasta contém o projeto sobre a loja de calcados "Passo a Passo". O objetivo é desenvolver os modelos: Conceitual, Lógico e Físico.</p>

## Mini Mundo  

<p>Imagine a loja de calçados "Passo a Passo", que oferece uma variedade de produtos, desde modelos casuais até opções mais sofisticadas. Para otimizar a gestão da loja e melhorar a experiência de compra, a empresa decidiu investir em um sistema que armazena dados essenciais sobre seus clientes, produtos e processos de venda.</p>
<p>Quando um cliente faz uma compra, o primeiro passo é registrar suas informações pessoais. Cada cliente precisa fornecer dados como nome, e-mails, telefones, endereço completo, que inclui rua, número, bairro, estado e CEP. Esses dados são fundamentais tanto para a comunicação com o cliente quanto para a realização da entrega. O sistema também mantém o controle sobre o estado e município do cliente, garantindo que as entregas sejam feitas de forma eficiente e sem erros.</p>
<p>Cada cliente pode realizar várias compras ao longo do tempo. Quando uma venda é realizada, os produtos escolhidos pelo cliente são registrados no sistema, e as informações sobre tamanho, cor e preço de cada item são detalhadas. O sistema também se preocupa em agrupar esses produtos em coleções, de acordo com a temporada ou o estilo, como "Coleção Primavera/Verão" ou "Coleção Casual". Isso ajuda a loja a organizar seus itens de maneira mais eficiente e permite que os vendedores façam recomendações personalizadas para os clientes com base nas coleções atuais</p>
<p>Para garantir que a loja tenha sempre os modelos mais vendidos ou os mais procurados, é crucial monitorar o estoque de cada produto. O sistema acompanha a quantidade em estoque. Cada produto é associado a um fabricante, que pode ser uma marca famosa ou um fornecedor local. O nome e a localização do fabricante também são armazenados, garantindo que a loja tenha informações suficientes para rastrear a origem dos produtos.</p>
<p>Além disso, o sistema mantém o controle detalhado de cada venda. Quando um cliente realiza uma compra, o valor total da transação e data são registrados. Cada venda é associada ao cliente que a fez, permitindo à loja acompanhar o histórico de compras e fornecer um atendimento mais personalizado no futuro.</p>
<p>Para que tudo isso funcione de forma integrada, o sistema garante que não haja conflito de dados entre as coleções, os produtos e os fabricantes. Cada produto pertence a uma única coleção, e cada fabricante fornece determinados itens. Quando um produto é vendido, o sistema verifica se há estoque disponível antes de processar a venda, evitando que o cliente compre um item que não pode ser entregue no prazo prometido.</p>
<p>Ao final, o sistema ajuda a Passo a Passo a manter a organização e o controle de seus dados essenciais: as informações dos clientes, os produtos, as coleções, o estoque e as vendas, criando um 
ambiente eficiente tanto para a gestão interna quanto para a experiência do cliente.</p>

## Entidades e Atributos

Abaixo estão as entidades principais do sistema e seus respectivos atributos: 

- **Cliente**: 
  - Atributos:
    - `Cod_cleinte`: Identificador único do cliente.
    - `Nome`: Nome do cleinte
    - `Telefones`: Atributo multivalorado, permitindo múltiplos contatos.
    - `E-mails`: tributo multivalorado, permitindo múltiplos endereços de e-mail.
    - `Endereço`: Atributo composto (Rua, número, bairro, estado, CEP).

- **Municipio**: 
  - Atributos:
    - `Cod_municipiio`: Identificador único do município.
    - `Nome`:Nome do município.

- **Estado**: 
  - Atributos:
    - `Sigla`: Sigla do estado.
    - `Nome`: Nome completo do estado.

- **Venda**: 
  - Atributos:
    - `Número`: Identificador único da venda.
    - `Data`: Data da venda.
    - `Total_venda`:Atributo derivado, calculado como quantidade * preço dos itens (Modelo conceitual).

- **Itens_Venda**:
  - Atributos:
    - `Numero_venda`: Chave primaria e estrangeria 
    - `Cod_produto`: Chave primaria e estrangeira
    - `preco`: Preço do produto na venda. 
    - `venda`: Venda associada ao item.

- **Produto**:
  - Atributos:
    - `Cod_produto`:Identificador único do produto
    - `Nome`:Nome do produto
    - `preco`:Valor do produto.
    - `Genero`: Gênero do produto.
    - `Cod_fabricante`:Identificador do fabricante
    - `Cod_modelo`:Identificador do modelo.
  
- **Fabricante**:
  - Atributos:
    - `Cod_fabricante`:Identificador único do fabricante.
    - `Nome`:Nome do fabricante.

- **colecao**:
  - Atributos:
    - `Cod_colecao`: Identificador da coleção.
    - `Nome`:Nome da coleção.

- **Estoque**: 
  - Atributos:
    - `Cod_produto`:Identificador do produto.
    - `numero`: Número de itens em estoque.
    - `quantidade`: Quantidade disponível.
    - `cor`: Cor do produto.

- **Modelo**:
  - Atributos:
    - `cod_modelo`: Identificador único do modelo.
    - `Nome`:Nome do modelo.

<p>Este projeto visa não apenas a implementação de um sistema de vendas, mas também a aplicação prática de conceitos de modelagem de dados.</p>

