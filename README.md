# Dados úteis para o Hackfest Contra a Corrupção

Uma lista não exaustiva mas útil de dados que já usamos ou vimos que é viável usar em edições passadas do Hackfest Contra a Corrupção.

<!-- toc -->

- [Prontos e já usados](#prontos-e-ja-usados)
    + [Receitas, licitações e despesas de municípios e estado da PB](#receitas-licitacoes-e-despesas-de-municipios-e-estado-da-pb)
  * [Presenças, votações e votos dos deputados federais na câmara](#presencas-votacoes-e-votos-dos-deputados-federais-na-camara)
  * [Discursos dos deputados federais na câmara](#discursos-dos-deputados-federais-na-camara)
  * [Gastos da Cota para Exercício da Atividade Parlamentar dos deputados federais](#gastos-da-cota-para-exercicio-da-atividade-parlamentar-dos-deputados-federais)
  * [Dados das empresas que prestaram serviço ao poder público na PB](#dados-das-empresas-que-prestaram-servico-ao-poder-publico-na-pb)
  * [Candidatos, seus bens e as doações que eles receberam nas eleições de 2012, 2014 e 2016](#candidatos-seus-bens-e-as-doacoes-que-eles-receberam-nas-eleicoes-de-2012-2014-e-2016)
  * [SICONV: uso de verba do governo federal por municípios e estados (e universidades, institutos, ...) via convênios](#siconv-uso-de-verba-do-governo-federal-por-municipios-e-estados-e-universidades-institutos--via-convenios)
  * [Prefeitos da PB com contas julgadas irregulares entre 2008 e 2016 pelo TCE-PB](#prefeitos-da-pb-com-contas-julgadas-irregulares-entre-2008-e-2016-pelo-tce-pb)
  * [Proposituras da Câmara Municipal de Campina Grande, PB](#proposituras-da-camara-municipal-de-campina-grande-pb)
- [Aparentemente prontos, mas não foram usados por nós](#aparentemente-prontos-mas-nao-foram-usados-por-nos)
  * [Dados abertos da prefeitura de João Pessoa](#dados-abertos-da-prefeitura-de-joao-pessoa)
  * [Cadastro de Empresas Inidôneas e Suspensas (CEIS)](#cadastro-de-empresas-inidoneas-e-suspensas-ceis)
  * [Cadastro de Entidades sem Fins Lucrativos Impedidas (CEPIM)](#cadastro-de-entidades-sem-fins-lucrativos-impedidas-cepim)
  * [Cadastro Nacional de Empresas Punidas (CNEP)](#cadastro-nacional-de-empresas-punidas-cnep)
  * [Dados sistematizados sobre parlamentares, seus gastos, parentes, empresas onde eles gastaram e discursos](#dados-sistematizados-sobre-parlamentares-seus-gastos-parentes-empresas-onde-eles-gastaram-e-discursos)
  * [Dados abertos do governo do Estado da PB](#dados-abertos-do-governo-do-estado-da-pb)
- [Possíveis e interessantes](#possiveis-e-interessantes)
  * [Atividade dos vereadores em João Pessoa, PB](#atividade-dos-vereadores-em-joao-pessoa-pb)
- [Contribuindo](#contribuindo)

<!-- tocstop -->

---

## Prontos e já usados

#### Receitas, licitações e despesas de municípios e estado da PB
?    | ! |
 --- | --|
*O que é* | Dump do SAGRES, o sistema que o Tribunal de Contas do Estado da PB usa para auditar os municípios e estado. |
*Formato* | csvs (6GB), e um banco MySQL no ar disponível para o hackfest. [O MER do BD é esse](etc/modelo-entidade-relacionamento-sagres.pdf)  |
*Dicas*   | Temos auditores do TCE como coaches no evento que entendem do riscado. Não temos todas as tabelas mencionadas no MER, pois algumas o TCE classifica como sensíveis. Uma descrição dos dados pode ser encontrada [aqui](etc/Sagres-DescricaoDados.pdf). |
*Projetos usando* | [contratospublicos.info](http://contratospublicos.info), [Destrinchando os gastos públicos](https://analytics-ufcg.github.io/licitacoes-pb/)  |

---

### Presenças, votações e votos dos deputados federais na câmara
?    | ! |
 --- | --|
*O que é* | Dados das presenças, das propostas votadas e dos votos individuais dos deputados federais. |
*Formato* | Em xml através de uma API da câmara ou em csvs [neste repositório](https://github.com/nazareno/dados-da-camara-federal). |
*Dicas*   | Tem bastante dado a mais na API da câmara, inclusive discursos dos deputados. |
*Projetos usando* | [House of Cunha](http://www.houseofcunha.com.br)  |

---

### Discursos dos deputados federais na câmara
?    | ! |
 --- | --|
*O que é* | Dados dos discursos de nossos representantes da câmara. |
*Formato* | Em xml através de uma API da câmara |
*Url*     | [Na API de dados abertos da câmara](http://www2.camara.leg.br/transparencia/dados-abertos/dados-abertos-legislativo/webservices/sessoesreunioes-2/obterinteiroteordiscursosplenario) |
*Dicas*   | Às vezes os exemplos da API não funcionam tal qual estão na página, mas mudando um pouco dá certo.  |
*Projetos usando* | [Retórica Parlamentar](http://retorica.labhackercd.net/), [Matéria do NEXO](http://cidadania20.com/projectos/deputados-federais-em-plenario/) |

---

### Gastos da Cota para Exercício da Atividade Parlamentar dos deputados federais
?    | ! |
 --- | --|
*O que é* | Cada deputado tem cerca de R$50 mil / mês para gastar em sua atividade parlamentar. A câmara abriu os dados de todos esses gastos para que a população fiscalize. |
*Formato* | A câmara disponibiliza arquivos XML, JSON, CSV e XLSX compactados para download contendo os dados relativos aos gastos parlamentares registrados na Câmara dos Deputados. |
*Url*     | Direto no [site da câmara](http://www2.camara.leg.br/transparencia/cota-para-exercicio-da-atividade-parlamentar/dados-abertos-cota-parlamentar) |
*Dicas*   | Tem bastante dado a mais na API da câmara, inclusive discursos dos deputados. |
*Projetos usando* | [House of Cunha](http://www.houseofcunha.com.br), [Serenata de Amor](http://serenatadeamor.org) |

---

### Dados das empresas que prestaram serviço ao poder público na PB
?    | ! |
 --- | --|
*O que é* | CEP, nome e funções no Cadastro Nacional de Atividade Empresarial para cada empresa que prestou algum serviço ou vendeu mercadoria ao poder público na PB  |
*Formato* | CSV |
*Url*     | Em um HD externo com o pessoal do MPPB no evento.  |
*Dicas*   | Temos construtoras vendendo remédios? |
*Projetos usando* | [contratospublicos.info](http://contratospublicos.info), [Destrinchando os gastos públicos](https://analytics-ufcg.github.io/licitacoes-pb/) |

---

### Candidatos, seus bens e as doações que eles receberam nas eleições de 2012, 2014 e 2016
?    | !  |
 --- | -- |
*O que é* | Detalhes demográficos, de bens, doações e gastos dos candidatos de 2016 e das eleições anteriores |
*Formato* | CSV |
*Url*     | http://www.tse.jus.br/hotSites/pesquisas-eleitorais/candidatos_anos/2016.html  |
*Dicas*   | Há um dicionário dos dados em pdf. O formato mudou um pouco ao longo dos anos, mas eles procuram manter a compatibilidade. Não é simples cruzar os nomes dos candidatos com os dos parlamentares na API da câmara.  |
*Projetos usando* | [De onde vem o dinheiro nas eleições de 2016?](https://nazareno.shinyapps.io/minha-cidade/), [Nossos vereadores, Campina Grande](http://www.vereadorescg.cc) |

---

### SICONV: uso de verba do governo federal por municípios e estados (e universidades, institutos, ...) via convênios
?    | !  |
 --- | -- |
*O que é* | Boa parte das obras estruturantes e grandes serviços dos municípios e estados é feito com verba federal obtida via convênios. O SICONV tem dados abertos detalhados sobre os convênios celebrados, licitações e pagamentos envolvidos, se a prestação de contas foi aceita ou houve problema, e o cronograma disso tudo. Tem também informação dizendo se a verba do convênio é resultante de uma emenda parlamentar de um deputado federal ou senador. |
*Formato* | CSVs |
*Url*     | http://portal.convenios.gov.br/download-de-dados  |
*Dicas*   | Há um MER na página. Os csvs são atualizados diariamente. Esses csvs são mais completos que a API de convênios. Prestação de contas rejeitada é sinal de que o convênio não foi executado corretamente. Deputados alocam verbas via emendas parlamentares que acabam sendo executadas como convênios. |
*Projetos usando* | [As Diferentonas](https://github.com/nazareno/diferentonas-server/), [Na emenda dos deputados](https://github.com/CelioBarros/NaEmendaDeputado), Quase todos [os apps que participaram do hackathon do MJ](https://github.com/LabPi) |

---

### Prefeitos da PB com contas julgadas irregulares entre 2008 e 2016 pelo TCE-PB
?    | ! |
 --- | --|
*O que é* | Lista dos gestores que tiveram sua prestação de contas anual rejeitada pelo Tribunal de Contas do Estado, que fiscaliza as contas dos municípios e do Estado da PB. |
*Formato* | csv |
*Url*     | [Neste link](etc/contas-irregulares-segundo-TCE.csv) |
*Dicas*   | Tem dados sobre pessoal na folha de pagamento da prefeitura, o que não é comum. |
*Projetos usando* |  |

---

### Proposituras da Câmara Municipal de Campina Grande, PB
     ?    | ! |
      --- | --|
*O que é* | Dados sobre proposituras dos vereadores, incluindo o que foi proposto, a categoria da propositura, o tema e alguns dados demográficos dos vereadores.  |
*Formato* | Banco postgres + crawler |
*Url*     | Os dados estão [nesse repo](https://github.com/augustoqm/cg-insights-data) e o crawler [nesse outro](https://github.com/augustoqm/cg-insights-data-gen)  |
*Dicas*   | Os dados não são abertos, mas estão públicos. O crawler e abordagem devem ser facilmente adaptáveis para outras câmaras que usem um software parecido de controle das proposituras. O de CG tem [essa cara](http://187.115.174.90:8080/ScanLexWeb/).  |
*Projetos usando* | www.vereadorescg.cc |

---

## Aparentemente prontos, mas não foram usados por nós

### Dados abertos da prefeitura de João Pessoa
?    | ! |
 --- | --|
*O que é* | Dados sobre pessoal, licitações, convênios, verba de publicidade e despesas/receitas da prefeitura. |
*Formato* | csvs ou sql |
*Url*     | http://transparencia.joaopessoa.pb.gov.br/download  |
*Dicas*   | Tem dados sobre pessoal na folha de pagamento da prefeitura, o que não é comum. |
*Projetos usando* |  |

---

### Cadastro de Empresas Inidôneas e Suspensas (CEIS)
?    | ! |
 --- | --|
*O que é* | Empresas e pessoas físicas que sofreram sanções pelos órgãos e entidades da administração pública das diversas esferas federativas. |
*Formato* | csv |
*Url*     | http://www.portaldatransparencia.gov.br/downloads/snapshot.asp?c=CEIS |
*Dicas*   |  |
*Projetos usando* |  |

---

### Cadastro de Entidades sem Fins Lucrativos Impedidas (CEPIM)
?    | ! |
 --- | --|
*O que é* | Entidades privadas sem fins lucrativos que estão impedidas de celebrar convênios, contratos de repasse ou termos de parceria com a administração pública federal |
*Formato* | csv |
*Url*     | http://www.portaldatransparencia.gov.br/downloads/snapshot.asp?c=CEPIM |
*Dicas*   |  |
*Projetos usando* |  |

### Cadastro Nacional de Empresas Punidas (CNEP)
?    | ! |
 --- | --|
*O que é* | Empresas que sofreram sanções previstas pela Lei nº 12.846/2013 (Lei Anticorrupção). As informações abrangem órgãos e entidades da administração pública das esferas federal, estadual e municipal. |
*Formato* | csv |
*Url*     | http://www.portaldatransparencia.gov.br/downloads/snapshot.asp?c=CNEP |
*Dicas*   |  |
*Projetos usando* |  |

---

### Dados sistematizados sobre parlamentares, seus gastos, parentes, empresas onde eles gastaram e discursos
?    | ! |
 --- | --|
*O que é* | Dados da câmara e de outras fontes, incluindo geolocalização das empresas onde parlamentares gastaram, seus parentes, seus assessores e mais coisa que parece bem legal, sistematizado pelo pessoal da Operação Serenata de Amor  |
*Formato* | csvs compactados como xz  |
*Url*     | https://github.com/datasciencebr/serenata-toolbox/ , também temos os dados no evento no hd externo chamado nuvem |
*Dicas*   |   |
*Projetos usando* | https://serenatadeamor.org |

---

### Dados abertos do governo do Estado da PB
?    | ! |
 --- | --|
*O que é* | Dados sobre receitas, despesas por tipo, diárias, passagens, licitações, dispensas de licitações, contratos,  aditivos e convênios do Estado da PB |
*Formato* | csv |
*Url*     | http://dados.pb.gov.br/ |
*Dicas*   |   |
*Projetos usando* |  |


## Possíveis e interessantes

### Atividade dos vereadores em João Pessoa, PB
?    | ! |
 --- | --|
*O que é* | O sistema de registro de proposituras da Câmara Municipal pode ser vasculhado e acompanhado por um crawler.  |
*Formato* | Hoje em HTML, mas em um formato simpático a crawlers.  |
*Url*     | [Este](http://177.200.32.195:9673/sapl/relatorios_administrativos/historicoTramitacoes/historicoTramitacoes_mostrar_proc?txt_dat_inicio_periodo=11%2F11%2F2016&txt_dat_fim_periodo=06%2F06%2F2017&lst_cod_unid_tram_dest=0&lst_tip_materia=0&lst_status=0&btn_materia_pesquisar=Pesquisar) pode ser um ponto de partida para o crawling.  |
*Dicas*   | Fizemos algo parecido no passado para a CMCG. Procura mais acima nesse documento.  |
*Projetos usando* |  |


## Contribuindo

Adoramos contribuições. Para adicionar um novo dado, copie o template abaixo, edite a seção e mande um pull request.

```
### Título
     ?    | ! |
      --- | --|
*O que é* |   |
*Formato* |   |
*Url*     |   |
*Dicas*   |   |
*Projetos usando* |  |
```
