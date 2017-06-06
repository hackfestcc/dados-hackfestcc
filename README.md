# Dados úteis para o Hackfest Contra a Corrupção

Uma lista não exaustiva mas útil de dados que já usamos ou vimos que é viável usar em edições passadas do Hackfest Contra a Corrupção.

## Prontos e já usados

#### Receitas, licitações e despesas de municípios e estado da PB

?    | ! |
 --- | --|
*O que é* | Dump do SAGRES, o sistema que o Tribunal de Contas do Estado da PB usa para auditar os municípios e estado. |
*Formato* | csvs (6GB), e um banco MySQL no ar disponível para o hackfest. **Link para o MER**  |
*Dicas*   | Temos auditores do TCE como coaches no evento que entendem do riscado. Não temos todas as tabelas mencionadas no MER, pois o TCE considerou algumas confidenciais. |
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

### Candidatos, seus bens e as doações que eles receberam nas eleições de 2012, 2014 e 2016
     ?    | ! |
      --- | --|
*O que é* | Detalhes demográficos, de bens, doações e gastos dos candidatos de 2016 e das eleições anteriores |
*Formato* | CSV |
*Url*     | http://www.tse.jus.br/hotSites/pesquisas-eleitorais/candidatos_anos/2016.html  |
*Dicas*   | Há um dicionário dos dados em pdf. O formato mudou um pouco ao longo dos anos, mas eles procuram manter a compatibilidade. Não é simples cruzar os nomes dos candidatos com os dos parlamentares na API da câmara.  |
*Projetos usando* | [De onde vem o dinheiro nas eleições de 2016?](https://nazareno.shinyapps.io/minha-cidade/), [Nossos vereadores, Campina Grande](http://www.vereadorescg.cc) |


## Prontos mas ainda não usados


## Possíveis e interessantes

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
