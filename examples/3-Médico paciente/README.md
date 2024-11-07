# Exercicio Médico Paciente

<p>Esta pasta contém o projeto sobre a Clínica "Vida Saudável". O objetivo é desenvolver os modelos: Conceitual, Lógico e Físico.</p>

## Mini Mundo
<p>A clínica "Vida Saudável" é conhecida por oferecer atendimento especializado em diversas áreas da medicina, como cardiologia, ortopedia e pediatria. A clínica deseja implementar um sistema para organizar os dados de seus pacientes, médicos, departamentos e consultas, além de gerenciar as prescrições de medicamentos e os laboratórios que os fabricam. Esse sistema ajudará a clínica a melhorar o atendimento e garantir que todas as informações dos pacientes e dos tratamentos estejam bem organizadas.</p>
<p>Cada paciente que frequenta a clínica tem um cadastro completo. Os dados armazenados incluem o nome completo, endereço (com rua, número, bairro, cidade, estado e CEP), telefones de contato (podendo ter um ou mais números) e email. Essas informações são essenciais para que a clínica possa entrar em contato com os pacientes e enviar lembretes de consultas e exames.</p>
<p>Os médicos da clínica têm um registro no sistema que inclui seu nome, CRM (registro no conselho de medicina), especialidade (como cardiologia, ortopedia, etc.) e o departamento em que atuam. Cada médico é associado a um ou mais departamentos, onde realiza seus atendimentos. Essa associação ajuda a clínica a organizar o quadro médico e alocar recursos de forma eficiente</p>
<p>A clínica é organizada por departamentos. Cada departamento tem um nome (como "Cardiologia" ou "Ortopedia"), um código de identificação, o andar onde está localizado e a quantidade de funcionários que trabalham nele.</p>
<p>Quando um paciente realiza uma consulta ou atendimento na clínica, todas as informações relevantes são registradas no sistema. Esse registro inclui a data e hora do atendimento, o diagnóstico dado pelo médico, uma análise clínica (com observações e dados relevantes) e o nome do médico responsável pelo atendimento. Esse histórico ajuda os médicos a entenderem o quadro clínico de cada paciente e a monitorarem o progresso de cada tratamento</p>
<p>Durante alguns atendimentos, o médico pode prescrever uma receita ao paciente. Cada receita inclui a data de emissão e orientações específicas sobre o uso dos medicamentos. Essa informação é essencial para o paciente seguir o tratamento corretamente e para a clínica manter o histórico de prescrições.</p>
<p>Os medicamentos prescritos pelos médicos também estão cadastrados no sistema da clínica. Cada medicamento possui informações como o nome do medicamento, a dosagem recomendada, o tipo de medicamento (por exemplo, comprimido, injeção, etc.), o princípio ativo (principal substância responsável pelo efeito do medicamento) e um link para a bula (para acesso a informações detalhadas sobre o uso e os possíveis efeitos colaterais).</p>
<p>Além disso, a clínica mantém um cadastro dos laboratórios que fabricam os medicamentos. Cada laboratório tem um nome e seu CNPJ. Dessa forma, é possível associar os medicamentos ao laboratório responsável, o que permite ao sistema organizar os dados dos fornecedores e garantir a rastreabilidade dos produtos.</p>

## Entidades
Abaixo estão algumas das entidades principais do sistema

- `Paciente`
- `Medico`
- `Departamento`
- `Atendiemnto`
- `Receita`
- `Medicamento`
- `Laboratorio`
<p>Este projeto não visa apenas o desenvolvimento de um sistema de gestão para a clínica, mas também proporciona uma aplicação prática dos conceitos de modelagem de dados, demonstrando como construir uma estrutura de dados eficiente e escalável para o setor de saúde.</p>