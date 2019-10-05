# O-Teu-Portal
P.O.O2019-2020
Titulo: O Teu Portal

Participantes:
Número	Nome
50036390	Maria Margarida Neno
50034581	Miguel Morais

Enquadramento:
Nos dias de hoje, o processo de gestão de Alunos, Docentes e Membros do Secretariado, em instituições de ensino, como por exemplo, Universidades e escolas, é algo que requer um elevado esforço por parte das pessoas do secretariado.
	Produtos como o Portal do Estudante e a Secretaria Virtual, são produtos que por vezes não são acopladores, pois muitas vezes são direcionados apenas e só para determinados membros da instituição de ensino, ou seja, são apenas direcionados para estudantes, ou apenas direcionados para docentes, e não para todos os membros integrantes da instituição. 
	Com o aparecimento da globalização, pensamos ser importante, ter uma plataforma que pudesse englobar todos os membros das instituições de ensino, pois será mais fácil e intuitivo para todos, fazer uso apenas e só de uma única plataforma, que será a mesma para todos. 
	Assim, O teu Portal, surge com a finalidade de resolver um dos grandes problemas existentes nos produtos que existem do mercado atual, ou seja, a inexistência de um produto que englobe todos os membros de uma instituição. 
O Teu Portal, é assim uma plataforma que permite realizar a gestão de todo o pessoal integrante de instituições de ensino, apenas e só através de uma única plataforma. 
Assim, O Teu Portal, irá estar disponível para diferentes tipos de utilizadores, tais como: Alunos, Docentes, Membros do Secretariado e Administradores (ambos com funções diferenciadas dentro da plataforma).
Para os alunos, será possível consultar/editar a sua informação pessoal, ver a lista dos restantes alunos e por fim consultar as suas avaliações.
Os docentes, para além de poderem consultar/ editar a sua própria informação pessoal, poderão ainda ver quais os cursos que lecionam, ver quais os alunos existentes, adicionar/remover alunos, e ainda realizar o lançamento de notas. 
No que diz respeito ao Pessoal do Secretariado, estes poderão também consultar/editar toda a sua informação pessoal, consultar a lista de alunos existentes na instituição, inserir/ remover alunos, e por fim, poderão ainda, adicionar/remover mensalidades. 
Por fim, os Administradores, poderão realizar todas as tarefas referidas anteriormente, á exceção do lançamento/ remoção de mensalidades, e poderão ainda adicionar/remover Docentes. 

Cenários:
Neste projeto estão presentes 4 utilizadores (Administradores; Alunos; Docentes; Pessoal do Secretariado) apesar dos mesmos partilharem funcionalidades nomeadamente: ver lista de alunos, editar de informação pessoal e inserir e remover alunos. A sua funcionalidade mais importante ou cenário principal é diferente.
•	Administrador: <Adicionar/Remover Docentes> - Ao entrar na sua conta este utilizador através do login será redirecionado para uma nova janela onde terá as opções adicionar e remover. Estas opções estarão visíveis através dos botões adicionar e remover docentes, respetivamente. Na situação do administrador querer adicionar um docente (clicar no botão “adicionar docente”), este terá que preencher a informação pessoal desse mesmo docente (nome; password; e-mail; contacto telefónico) e por fim carregar no botão “adicionar docente” desta nova janela. Na situação do administrador querer remover um docente (clicar no botão “remover docente”), este será confrontado com uma lista de todos os docentes existentes, ao encontrar o docente que e selecioná-lo terá que carregar no botão “remover docente” desta nova janela.  
•	Alunos: <Consultar notas> - Ao entrar na sua conta este utilizador através do login será redirecionado para uma nova janela onde terá a opção consultar notas. Esta opção estará visível através do botão “consultar notas”. Ao clicar no botão “consultar notas”, este visualizará as notas das disciplinas a que está inscrito numa nova janela.
•	Docentes: <Lançar notas> - Ao entrar na sua conta este utilizador através do login será redirecionado para uma nova janela onde terá a opção lançar notas. Esta opção estará visível através do botão “lançar notas”. Ao clicar no botão “lançar notas”, este visualizará uma lista de alunos que tem a seu encargo onde terá que aceder ao “perfil” de cada um dos alunos e preencher o campo “avaliação”, situação esta que irá despoletar uma janela diferente e por fim carregar no botão “lançar notas” desta nova janela.
•	Pessoal do Secretariado: <Adicionar/Remover mensalidades> - Ao entrar na sua conta este utilizador através do login será redirecionado para uma nova janela onde terá as opções adicionar e remover. Estas opções estarão visíveis através do botão “adicionar e remover mensalidades”. Ao clicar no botão “adicionar e remover mensalidades”, este visualizará uma lista de alunos inscritos no estabelecimento de ensino e terá que aceder ao “perfil” de cada um dos alunos e preencher o campo “mensalidade” e introduzir o valor da mensalidade, situação esta que irá despoletar uma janela diferente e por fim carregar no botão “adicionar e remover mensalidades” desta nova janela. Quando o aluno efetua o pagamento, este utilizador visualizará a mesma lista de alunos inscritos no estabelecimento de ensino só que agora preencherá o campo “mensalidade” e introduzir o valor da mensalidade, neste caso 0 situação esta que irá despoletar uma janela diferente.

Cenários secundários:
•	Administrador: <Editar informação pessoal> - Ao entrar na sua conta este utilizador através do login será redirecionado para uma nova janela onde terá a opção editar administrador. Esta opção estará visível através do botão “editar administrador”. Ao clicar no botão “editar administrador”, este visualizará, numa nova janela toda a informação que poderá alterar, nomeadamente nome; e-mail; password e por fim carregar no botão “editar administrador” desta nova janela, fazendo assim update.
•	Alunos: <Editar informação pessoal> - Ao entrar na sua conta este utilizador através do login será redirecionado para uma nova janela onde terá a opção editar aluno. Esta opção estará visível através do botão “editar aluno”. Ao clicar no botão “editar aluno”, este visualizará, numa nova janela toda a informação que poderá alterar, nomeadamente nome; e-mail; password; morada e número de contribuinte e por fim carregar no botão “editar aluno” desta nova janela, fazendo assim update.
•	Docentes: <Inserir/Remover alunos> - Ao entrar na sua conta este utilizador através do login será redirecionado para uma nova janela onde terá as opções inserir e remover. Estas opções estarão visíveis através dos botões inserir e remover alunos, respetivamente. Na situação do docente querer inserir um aluno (clicar no botão “inserir aluno”), este terá que escolher um aluno de uma lista de alunos dos quais leciona, isto tudo numa janela diferente e por fim carregar no botão “inserir aluno” desta nova janela, fazendo assim update. Na situação do docente querer remover um aluno (clicar no botão “remover aluno”), este terá que escolher um aluno de uma lista de alunos dos quais leciona, isto tudo numa janela diferente e por fim carregar no botão “remover aluno” desta nova janela, fazendo assim update.
•	Pessoal do Secretariado: <Inserir/Remover alunos> - Ao entrar na sua conta este utilizador através do login será redirecionado para uma nova janela onde terá as opções inserir e remover. Estas opções estarão visíveis através dos botões inserir e remover alunos, respetivamente. Na situação deste utilizador querer inserir um aluno (clicar no botão “inserir aluno”), este terá que escolher um aluno de uma lista de alunos, alunos estes que frequentam esse estabelecimento de ensino, isto tudo numa janela diferente e por fim carregar no botão “inserir aluno” desta nova janela, fazendo assim update. Na situação deste utilizador querer remover um aluno (clicar no botão “remover aluno”), este terá que escolher um aluno de uma lista de alunos, alunos estes que frequentam esse estabelecimento de ensino, isto tudo numa janela diferente e por fim carregar no botão “remover aluno” desta nova janela, fazendo assim update.

