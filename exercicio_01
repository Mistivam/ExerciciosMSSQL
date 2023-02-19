--Exercicio 01

==tabela dimensão

CREATE TABLE tb_dados_funcionario(
	matricula INTEGER PRIMARY KEY IDENTITY (1,1) NOT NULL,
	nome VARCHAR (100) NOT NULL,
	data_nascimento DATE NOT NULL,
	nacionalidade VARCHAR (50) NOT NULL,
	estado_civil VARCHAR (50) NOT NULL,
	endereco VARCHAR (100) NOT NULL,
	telefone VARCHAR (20) NOT NULL,
	data_admissao DATE NOT NULL	
	);

--tabelas de fato

CREATE TABLE tb_cargos_ocupados(
	cargo VARCHAR (50) NOT NULL,
	data_inicio DATE NOT NULL,
	data_fim DATE NOT NULL,
	matricula INTEGER NOT NULL	
	);

CREATE TABLE tb_dependentes(
	nome_dependente VARCHAR (100) NOT NULL,
	data_nascimento DATE NOT NULL,
	matricula INTEGER NOT NULL	
	);

ALTER TABLE tb_cargos_ocupados ADD CONSTRAINT FK_tb_dados_funcionario_cargos FOREIGN KEY (matricula)
	REFERENCES tb_dados_funcionario (matricula);

ALTER TABLE tb_dependentes ADD CONSTRAINT FK_tb_dados_funcionario_dependentes FOREIGN KEY (matricula)
	REFERENCES tb_dados_funcionario (matricula);


	
	
