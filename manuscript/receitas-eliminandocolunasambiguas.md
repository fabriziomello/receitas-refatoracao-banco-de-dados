# Eliminando Colunas Ambíguas #
Conhecido originalmente como *"Multipurpose Colum"* ([Ambler](http://www.agiledata.org/essays/databaseRefactoringSmells.html)) indica que se uma coluna for utilizada para vários fins, é provável que exista um código extra para garantir que a mesma seja usada corretamente e, muitas vezes, verificando valores de uma ou mais colunas.

1. **Ingredientes**
	1. Ferramentas
		* [PostgreSQL](http://www.postgresql.org)
		* [pgTap](http://www.pgtap.org)

	1. Técnicas
		* [Testes de Bancos de Dados](http://www.agiledata.org/essays/databaseTesting.html)
		* [Refatoração de Banco de Dados](http://fabriziomello.github.io/blog/2013/06/10/database-refactoring)

	1. Mecânica
		1. Seguindo o princípio [KISS](https://pt.wikipedia.org/wiki/Keep_It_Simple) identifique 1 (uma) coluna com informação ambígua
		2. Garanta que esta ambiguidade tenha cobertura razoável de casos de testes
		3. Caso a cobertura de testes não esteja razoável então adicionar mais casos (escrever testes com pgTap)
		4. Aplicar técnicas de refatorações de banco de dados

1. **Aplicando a receita**
