# Oscars-goes-to...
![oscars](https://github.com/LucasSilva77/Oscars-goes-to/assets/125465336/e30d2620-d66e-4f14-97c7-30e93c95f0c9) 

## Muito bem, Pessoal...
Hoje vamos trabalhar com o Oscar. A ideia de premiar ou ser premiado é para reconhecer:

Reconhecer uma qualidade Reconhecer um atributo Reconhecer o esforço... Reconhecer sempre.

Nem todos os prêmios são merecidos e nem todos que merecem ganham prêmios. Então vale mesmo a pena, premiar?

## Quantas vezes Natalie Portman foi indicada ao Oscar? 
Código: SELECT NAME, winner FROM movies WHERE NAME LIKE "%Natalie Portma%"<br/>
Resposta: Ela foi indicada 3 vezes ao Oscar

## Quantos Oscars Natalie Portman ganhou? 
Código: SELECT NAME, winner FROM movies WHERE NAME LIKE "%Natalie Portma%"<br/>
Resposta: Ela venceu apenas 1 vez o Oscar

## Amy Adams já ganhou algum Oscar? 
Código: SELECT NAME, winner FROM movies WHERE name LIKE "%Amy Adams%";<br/>
Resposta: Ela Nunca ganhou o Oscar

## A série de filmes Toy Story ganhou um Oscar em quais anos? 
Código: SELECT film, winner, year_ceremony FROM movies WHERE film LIKE "%Toy Story%";<br/>
Resposta: 2011 e 2020

## Quem tem mais Oscars: a categoria "Melhor Ator" ou "Melhor Filme"? 
Código: SELECT "Filmes" as category, count() as winner FROM movies WHERE category LIKE '%FILM%' and winner = "True" UNION SELECT "actor" as category, count() as winner FROM movies WHERE category LIKE '%ACTOR%' and winner = "True";<br/>
Resposta: A Categoria "Melhor Filme"

## O primeiro Oscar para melhor Atriz foi para quem? Em que ano? 
Código: SELECT name, year_ceremony, winner FROM movies WHERE category LIKE "%ACTRESS%" and winner = 1;<br/>
Resposta: Foi para Janet Gaynor em 1928

## Na coluna/campo Winner, altere todos os valores com "True" para 1 e todos os valores "False" para 0 Código:
UPDATE movies SET winner = 1 WHERE winner = "True"; UPDATE movies SET winner = 0 WHERE winner = "False";<br/>

## Em qual edição do Oscar "Crash" ganhou o prêmio principal?
Código: SELECT film, winner, ceremony, category FROM movies WHERE film = "Crash" AND winner = 1;<br/>

Resposta: FILM EDITING, BEST PICTURE e WRITING

## Bom... dê um Oscar para um filme que merece muito, mas não ganhou.
Código: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2016', '2017', '1', 'Best Film', 'Conrad Vernon', 'Sausage Party', 'True');<br/>

## O filme Central do Brasil aparece no Oscar?
Código: SELECT film FROM movies where film like "%Central do Brasil%";<br/>

Resposta: Não Aparece

## Inclua no banco 3 filmes que nunca nem foram nomeados ao Oscar, mas que na sua opinião, merecem. 
Código 1: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2007', '2020', '92', 'HONORARY AWARD', 'José Padilha', 'Tropa de Elite', 'True');<br/>
Código 2: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2014', '2020', '92', 'VISUAL EFFECTS', 'Wes Ball', 'Maze Runner: Correr ou Morrer', 'False');<br/>

Código 3: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2013', '2020', '92', 'MUSIC (Original Song)', 'Guillermo del Toro', 'Círculo de Fogo', 'True');<br/>

## Crie uma nova categoria de premiação. Qualquer prêmio que você queira dar. Agora vamos dar esses prêmios aos filmes que você cadastrou na questão acima.
Código: UPDATE movies SET category = 'BEST SCREENPLAY' WHERE category = 'HONORARY AWARD';

## Qual foi o primeiro ano a ter um prêmio do Oscar?
Código: SELECT year_ceremony FROM movies;<br/>
Resposta: O Primeiro ano foi 1928

## Pensando no ano em que você nasceu: Qual foi o Oscar de melhor filme, Melhor Atriz e Melhor Diretor?
Código: SELECT film, category, year_ceremony, ceremony FROM movies WHERE year_ceremony = "2001";<br/>
Melhor Filme: Gladiator

Melhor Atriz: Julia Roberts<br/>

Melhor Diretor: Steven Soderbergh<br/>

## Agora procure 7 atrizes que não sejam americanas, europeias ou brasileiras. Vamos cadastrá-los no nosso banco, mas eles ainda não ganharam o Oscar. Só foram nomeados. 
Código 1: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2009', '2010', '1', 'ACTOR', 'Jamie Chung', 'Dragonball Evolution', 'False');<br/>
Código 2: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2021', '2021', '1', 'ACTOR', 'Jessica Henwick', 'Matrix Resurrections', 'False');<br/>

Código 3: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2001', '2002', '1', 'ACTOR', 'fatoumata diawara', 'Sia, The Dream of the Python', 'False');<br/>

Código 4: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2003', '2004', '1', 'ACTOR', 'charlize theron Chan', 'Monster - Desejo Assassino', 'False');<br/>

Código 5: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2010', '2011', '1', 'ACTOR', 'Zhao Tao', 'Memorias de Xangai', 'False');<br/>

Código 6: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('1988', '1988', '1', 'ACTOR', 'Dolly Rathebe', 'Mapantsula', 'False');<br/>

Código 7: INSERT INTO movies (year_film, year_ceremony, ceremony, category, name, film, winner) VALUES ('2019', '2019', '1', 'ACTOR', 'Jackson Yee', 'Dias Melhores', 'False');<br/>

## Agora vamos falar da sua vida. Me diga o nome de uma pessoa que você admira e o que ela fez na sua vida. Agora me diz: Quê prêmio essa pessoa merece?
<br/>Resposta: Minha mãe, ela ganharia um oscar de melhor pessoa do mundo e tambem de melhor mãe
