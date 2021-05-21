Neste repositório, pretendo colocar algumas análises de dados abertos que comecei a fazer utilizando diversas ferramentas, mas principalmente jupyter notebooks.

Apesar das informações estarem abertas, são de acesso um tanto complicado. No caso da dívida da união, até existe um painel dinâmico - ainda assim as informações não são tão diretas.

Os dados da união foram retirados de https://www.gov.br/pgfn/pt-br/assuntos/divida-ativa-da-uniao/dados-abertos 
Acesse para conseguir os dados completos, já que só consigo colocar os arquivos com menos de 25MB aqui.

Sobre a pasta FGTS: apenas 1 arquivo era maior que 25MB, mas não diz respeito a nenhuma UF... A sigla que o arquivo tinha era "NA" - correspondendo a "nacional". Assim, precisei verificar se aquele arquivo não tinha entradas repetidas comparado ao total das UF, o que se mostrou sendo o caso. O arquivo final que junta todas as entradas da dívida de FGTS excluindo as duplicadas também é superior a 25MB, então também não está no repositório, infelizmente. Tal arquivo não possui valores na coluna "UF responsável", herdado do csv nacional, então é preciso converter esse vazio para strings vazios toda vez que o read_csv é utilizado com ele.

20/05/2021 - Com as adições de hoje, considero satisfatório esse início de projeto. Novas adições sempre podem surgir mais tarde, especialmente com dados futuros, mas do ponto de vista técnico, não preciso mais priorizar tanto a adição de análises aqui.
