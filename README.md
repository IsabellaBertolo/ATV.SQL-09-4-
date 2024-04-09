# ATV.SQL-09-4-

----ATIVIDADE_3
-- adicionar coluna 'sexo' e atribuir os devidos valores a cada aluno
UPDATE alunos
SET sexo = 'M';

UPDATE alunos
SET sexo = 'F'
WHERE id IN (1, 2, 4, 5, 6, 7, 9, 11, 12, 13, 15, 17, 18, 19, 20, 22, 23, 24, 27, 28);

-- calcular média de todas as idades de todos os alunos
SELECT AVG(idade) AS media_idade FROM alunos;

-- somar todas as idades de todos os alunos
SELECT SUM(idade) AS soma_idades FROM alunos;

-- calcular média das idades das alunas e alunos separadamente
SELECT AVG(idade) AS media_idade
FROM alunos
WHERE sexo = 'F';

SELECT AVG(idade) AS media_idade
FROM alunos
WHERE sexo = 'M';

-- somar as idades das alunas e alunos separadamente
SELECT SUM(idade) AS soma_idades
FROM alunos
WHERE sexo = 'F';

SELECT SUM(idade) AS soma_idades
FROM alunos
WHERE sexo = 'M';
