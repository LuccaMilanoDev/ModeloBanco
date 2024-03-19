Nome: Lucca Milano Casado dos Santos ---
Modelo escolhido: Biblioteca ----
Entidades e atributos:
Usuario: Endereço, cpf(chave), telefone,nome(nome e sobrenome) e dataInscrição. ----
Estudante(extensão de usuario): carteira de estudante(chave) e desconto(estudante ganha desconto). ----
ClientePadrão(extensão de usuario): idCliente(chave). ----
Livros: nome (chave), multaAtraso,dataCompra(data onde foi feito o emprestimo), dataEntrega(data para receber de volta o livro) e sinopse. ----
Funcionario: nome(nome e sobrenome), cpf, funcionarioID(chave) e salario. ----
Autor: nome(chave). ----
Pagamento: valor,idPagamento(chave),Statusdesconto(caso a pessoa for estudante para efetuar desconto) e statusMulta(que ve se a multa precisa ser aplicada ou não).

Criei uma extensão de usuario pois julguei necessario num ambiente de biblioteca colocar um cliente tipo estudante para aplicar um desconto nos livros. Além disso criei entidade pagamento para fazer o pagamento dos livros. Criei também a entidade funcionario que é o funcionario da biblioteca que genrencia os livros 
