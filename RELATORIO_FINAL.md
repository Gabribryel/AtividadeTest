Relatório Final de Qualidade e Testes Web

Projeto Avaliado: AtividadeTest (https://gabribryel.github.io/AtividadeTest/)
Repositório: `https://github.com/gabribryel/AtividadeTest`

Líder de Qualidade (QA Lead): Roger Matos do Nascimento
Testador UI/UX & Usabilidade: Gabriel Yury Bezerra Monteiro
Testador de Performance & Técnico: Gabriel Yury Bezerra Monteiro


1. Resumo Executivo
Este documento apresenta os resultados consolidados do ciclo de testes realizados na aplicação web hospedada via GitHub Pages (`https://gabribryel.github.io/AtividadeTest/`) A avaliação seguiu os critérios estabelecidos no `PLANO_DE_TESTES.md`, abrangendo auditorias técnicas de desempenho, acessibilidade, boas práticas, SEO e validação visual de responsividade.

De modo geral, a aplicação demonstrou excelente conformidade em Boas Práticas (96) e Acessibilidade (93), atingindo a faixa verde de aprovação. Entretanto, foram identificadas oportunidades de melhoria nas métricas de Performance e SEO, além de ajustes pontuais de interface, todos devidamente documentados na aba Issues do repositório.


2. Resultados do Google Lighthouse (Antes vs. Proposta de Correção)

Abaixo estão os indicadores coletados nas auditorias do Google Lighthouse (faixa de pontuação: `0–49` Vermelho / `50–89` Laranja / `90–100` Verde):

Auditoria 1 (Desktop / Execução Base)
Métrica | Nota Inicial (Antes) | Nota Esperada (Após Correções) | Classificação Atual |

Performance | 79 | 92+ |  Atenção (50–89) |
Accessibility | 93 | 98+ |  Aprovado (90–100) |
Best Practices | 96 | 100 |  Aprovado (90–100) |
SEO | 82| 95+ |  Atenção (50–89) |

Auditoria 2 (Mobile / Execução Secundária)
Métrica | Nota Inicial (Antes) | Nota Esperada (Após Correções) | Classificação Atual |

Performance | 75 | 90+ |  Atenção (50–89) |
Accessibility | 93 | 98+ |  Aprovado (90–100) |
Best Practices | 96 | 100 |  Aprovado (90–100) |
SEO | 82 | 95+ |  Atenção (50–89) |

 Diagnóstico Técnico: A queda de pontuação em Performance (79 e 75)[cite: 1, 2] está associada ao tempo de carregamento dos recursos visuais e renderização inicial. Já a nota de SEO (82) reflete a ausência de metadados descritivos (`meta description`) no cabeçalho HTML da página.


3. Matriz de Bugs e Melhorias Encontradas

Todas as ocorrências identificadas durante as inspeções no Lighthouse, WAVE e Chrome DevTools foram registadas como Issues neste repositório:

Issue | Categoria | Descrição do Problema / Melhoria | Severidade | Ambiente | Status |

[#1](issue) | Performance | Otimização de imagens e recursos estáticos para elevar o índice de Performance (atualmente em 75–79) | Média | Mobile / Desktop | Aberta |
[#2](issue) | SEO | Inclusão da tag `<meta name="description">` no `<head>` para melhorar a indexação e elevar a nota de SEO (atualmente em 82) | Baixa | Todos | Aberta |
[#3](issue) | UI / Design | [Ex: Ajuste de espaçamento/quebra de layout em telas mobile menores que 390px]. | Média | Mobile | Aberta |
[#4](issue) | Acessibilidade | [Ex: Revisão de contraste de cores / atributos `alt` apontados pela ferramenta WAVE]. | Baixa | Todos | Aberta |

(Nota: Caso o grupo tenha encontrado mais ou menos ocorrências, ajuste as linhas da tabela acima conforme as Issues realmente abertas no GitHub).


4. Conclusão e Recomendações
A aplicação `AtividadeTest` apresenta uma base técnica sólida, destacando-se pela pontuação de 96 em Boas Práticas e 93 em Acessibilidade; Para atingir a excelência (notas acima de 90 em todos os pilares), recomenda-se priorizar a resolução das Issues de Performance (compressão de ativos e carregamento assíncrono) e SEO (adição de meta tags descritivas), seguidas pelos ajustes finos de layout responsivo.
