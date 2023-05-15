# Projeto Integrador - ParkItU

Documentação para o desenvolvimento do Projeto Integrador do Curso de Técnico em Desenvolvimento de Sistemas para a Internet Integrado ao Ensino Médio do IFC - Campus Araquari.

Estudantes: [Eduardo Barbaro](github.com/dudubarbaro) e [Brunno Duarte da Cunha](https://github.com/BrunnoDC).

Links do projeto:

-   [Documentação](github.com/dudubarbaro/pi-modelo)
-   [Backend]()
-   [Frontend]()

# Empréstimo

Gerenciamento de um estacionamento

  O nossa empresa, ParkItU, está crescendo, devido a procura por vagas para os veículos de nossa região. Recentemente, contratamos dois funcionários para o gerenciamento e desenvolvimento digital.
  Assim, atualmente, conseguimos concentrar nossos esforços para melhorar a gestão de nosso gerenciamento. Para isso, queremos adquirir um sistema de controle de que nos permita monitorar a entrada e saída de veículos do nosso estabelecimento. Como nossa intenção é melhorar a gestão do negócio, é muito importante que consigamos ter relatórios, como por exemplo, numero de ingressos e egressos mensais.

# Situação Problema

  O cliente conhece nosso local por meio de nossos conteúdos digitais em nossas redes sociais, indicações ou até por propagandas/ convênios e folhetos impressos. A fim de deixar seu carro em segurança , com a ideia de alocar, cotar ou apenas verificar uma vaga, ele nos contacta e vai até nós.
  No local, ele é bem recepcionado pelos donos, apresentamos as vagas disponíveis, o fidelizamos e o deixamos tranquilo para sair para seus compromissos e deixar seu veículo em segurança.
  Na volta, nós atualizamos nossa cotação e o preço é lançado num recibo. Com o pagamento finalizado, acomprovante retirado, o dono do veículo estará liberado para sair com seu automóvel.
  Com isso notamos alguns problemas em relação ao gerenciamento dos veículos no pátio, controle de entrada e saída dos automóveis, controle de clientes e divulgações para vendas em redes sociais, por serem muito fechadas ao seu público alvo nativo. 
  Já atuando na resolução desses problemas, escolhemos por obter o desenvolvimento de um software de gerenciamento para nos ajudar a manter o maior controle e segurança dos veículos de nossos clientes, principalmente, com um domínio próprio na internet, uma maior liberdade de divulgação e modernidade à nossa empresa.

# Descrição da proposta

O desenvolvimento do predicado software advém da necessidade da situação-problema que se caracteriza com a relação ao gerenciamento dos veículos no pátio, controle de entrada e saída dos automóveis, controle de clientes e divulgações para vendas em redes sociais, por serem muito fechadas ao seu público alvo nativo.
Para isso o sistema terá seu foco no gerenciamento de veículos e clientes. O sistema permitirá a adição e a remoção de veículos, a visualização e controle do patio e das vagas, relatório de entrada e saída de veículos e os registros dos clientes. Dois níveis de usuário: Admin e Cliente. O Admin terá acesso as telas de gerenciamento, controle, relatório e registro de venda. O usuário Cliente terá acesso a tela de visualização das vagas disponíveis e do status referente ao seu veículo.

# Regras de Negócio

**RN01 - Cadastro de veículos:** Para validar a alocação de um veículo, é de suma importância ter uma vaga disponível. <br />
**RN02 - Adicionar uma veículo:**  Para adicionar um veículo, é preciso que o veículo esteja cadastrado no sistema e que seu status esteja como aprovado.<br />
**RN03 - Cadastro de usuários:** Os usuários precisam realizar o cadastro para fazer a requisição de uma vaga.<br />
**RN04 - Reservar vaga:** Para realizar o pedido de uma vaga, apenas com usuários cadastrados e nenhuma outra vaga em aberto.<br />
**RN05 - Registro de empréstimo:** O Administrador deve possuir acesso aos gerenciamentos de veículos<br />
**RN06 - Desfazer espréstimo em aberto:** O usuário que possuir o status de sua vaga em aberto deverá desfazer sua pendência.<br />
**RN07 – Impressão da vaga:** Com as informações da vaga registrada, o adminstrador deve enviar ao usuário para aprovação, e caso o usuário aprovar, o administrador deve solicitar a sua assinatura online para aprovar a execução do serviço.<br />
**RN08 – Abertura de OS:** Com a reserva aprovada pelo usuário, o administrador deverá receber os dados do usuário e da venda em um novo formulário, para o gerenciamento interno, realizando a abertura da vaga.<br />
**RN09 – Gerenciamento de fluxo de vagas e veículos:** O gerenciamento de fluxo de veículos  será permitido somente para o administrador.

# Requisitos Funcionais

**RF01 - Registro de veículos:** O sistema deve permitir o registro de informações sobre os veículos que entram no estacionamento, como placa, modelo, cor e hora de entrada.<br />
**RF02 - Controle de acesso:** O sistema deve ser capaz de controlar o acesso de veículos ao estacionamento, permitindo a entrada apenas de veículos autorizados e registrando informações sobre a hora de entrada.<br />
**RF03 - Alocação de vagas:** O sistema deve atribuir vagas disponíveis aos veículos que entram no estacionamento, garantindo uma alocação eficiente e evitando o uso indevido de vagas.<br />
**RF04 - Cobrança de tarifas:** O sistema deve calcular e registrar as tarifas de estacionamento com base na duração da estadia do veículo.<br />
**RF05 - Pagamento:** O sistema deve fornecer opções de pagamento para os clientes, como dinheiro, cartão de crédito ou aplicativos de pagamento móvel. Além disso, deve gerar recibos ou comprovantes para as transações efetuadas.<br />
**RF06 - Gerenciamento de vagas:** O sistema deve permitir o monitoramento e o gerenciamento das vagas disponíveis, informando quais estão ocupadas e quais estão livres, facilitando a localização de vagas para os motoristas.<br />
**RF07 - Relatórios e estatísticas:** O sistema deve ser capaz de gerar relatórios e estatísticas sobre a ocupação do estacionamento, a receita gerada, entre outros dados relevantes para a gestão do estacionamento.

# Requisitos Não Funcionais

**RNF01 - Confiabilidade:** O sistema deve ser confiável, garantindo a disponibilidade e a integridade dos dados registrados, além de operar sem falhas frequentes.<br />
**RNF02 - Desempenho:** O sistema deve ser capaz de lidar com um grande número de veículos, processando as transações de entrada, saída e pagamento de forma rápida e eficiente.<br />
**RNF03 -Segurança:** O sistema deve garantir a segurança das informações dos clientes, como dados pessoais e informações de pagamento, utilizando técnicas adequadas de criptografia e controle de acesso.<br />
**RNF04 -Usabilidade:** O sistema deve ser fácil de usar e intuitivo, tanto para os funcionários responsáveis pela operação do estacionamento quanto para os clientes que utilizam o serviço.<br />
**RNF05 - Escalabilidade:** O sistema deve ser capaz de lidar com um aumento na demanda sem comprometer o desempenho, permitindo a expansão do estacionamento sem grandes dificuldades.<br />
**RNF06 - Integração:** O sistema deve ser capaz de se integrar com outros sistemas, como sistemas de controle de acesso, sistemas de pagamento e sistemas de gestão financeira.<br />
**RNF07 - Manutenibilidade:** O sistema deve ser facilmente mantido e atualizado, permitindo a correção de falhas, a incorporação de novas funcionalidades e a aplicação de melhorias quando necessário.
