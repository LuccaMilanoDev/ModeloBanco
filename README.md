Nome: Lucca Milano Casado dos Santos ---
Modelo escolhido: Biblioteca ----
Entidades e atributos:
Usuario: Endereço, cpf(chave), telefone,nome(nome e sobrenome) e dataInscrição.---	  
Estudante(extensão de usuario): carteira de estudante(chave) e desconto(estudante ganha desconto).---
ClientePadrão(extensão de usuario): idCliente(chave).--- 	
Livros: nome (chave), multaAtraso,dataCompra(data onde foi feito o emprestimo), dataEntrega(data para receber de volta o livro) e sinopse.--- 
Funcionario: nome(nome e sobrenome), cpf, funcionarioID(chave) e salario.---
Autor: nome(chave).---
Pagamento: valor,idPagamento(chave),Statusdesconto(caso a pessoa for estudante para efetuar desconto) e statusMulta(que ve se a multa precisa ser aplicada ou não).---

Criei uma extensão de usuario pois julguei necessario num ambiente de biblioteca colocar um cliente tipo estudante para aplicar um desconto nos livros. Além disso criei entidade pagamento para fazer o pagamento dos livros. Criei também a entidade funcionario que é o funcionario da biblioteca que genrencia os livros 

Modelo(Atualizado)
No novo modelo fiz algumas alterações sugeridas pelo professor. 
Troquei a chave de usuario para IDusuario para ficar mais facil e não exigir que o usuario tenha cpf alem de ter adicionado mais uma chave que foi o email.
Liguei usuario ao emprestimo dessa forma permitindo que qualquer tipo de usuario possa fazer o empretismo e coloquei como opção de ele fazer emprestimo ou não (0,N) ou seja 0 ou mais emprestimos. Usuario agora esta ligado a efetua de efetuar pagamento pois ele tem ligação direta com o pagemento coloquei como cardinalidade (0,N) pois pode ter nenhum pagamento ou mais.
Adicionei atributos a emprestimo para quando fizer emprestimo esteja salvo a data que ele realizou o emprestimo e também salvo a data que ele deve entregar, realoquei o multaAtraso para emprestimo pois a multa esta ligado as datas.
Troquei a cardinalidade entre pagamento e livros conforme foi recomendado podendo assim o usuario escolher um ou varios livros mas ocorre apenas um pagamento.
