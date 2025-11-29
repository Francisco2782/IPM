# Proposta de interface (1ª fase)
# Análise de Usabilidade do protótipo em Figma

Interface Pessoa-Máquina 

Licenciatura em Engenharia Informática - Universidade do Minho

19 de outubro de 2025  


[Visualizar Protótipo no Figma](https://www.figma.com/proto/7R7Tmq2f0DfOaMFEZyhSoR/Airbnb?node-id=0-1&t=mqvJDh8uQHaQStXs-1)
---
## Objetivo da Interface

O protótipo visa criar uma interface de visualização de dados da plataforma InsideAirbnb, focada em apoiar três tipos de utilizadores (investigador, gestora pública e ativista) na análise e comunicação de dados sobre o impacto do alojamento local.  
O design prioriza acessibilidade, clareza e flexibilidade, permitindo explorar dados temporais, geográficos e comparativos de forma intuitiva.

---
## Necessidades dos Perfis de Utilizador

Cada perfil representa um tipo distinto de utilizador com objetivos, contextos e competências específicas, que foram considerados na realização deste protótipo. 

##  Perfil 1 — Investigador de Pós-Doutoramento 

**Necessidades Principais**
1.  **Análise temporal detalhada** (séries temporais de vários meses)  
2.  **Filtros complexos** por tipo de propriedade,localização e preço
3.  **Exportação de resultados** em formatos standard (CSV, JSON)
   
**Implicações para a interface proposta**

- Foi criada uma frame dedicada à análise detalhada de séries temporais, permitindo a visualização e comparação de dados ao longo de períodos extensos.

- A interface oferece uma variedade de filtros avançados, aplicáveis à pesquisa por localização, tipo de propriedade, intervalo de preços e intervalo de tempo.

- Desenvolveu-se uma frame de exportação de dados da localidade selecionada, com suporte aos formatos CSV e JSON, bem como a opção de descarregar dados detalhados ou versões resumidas conforme a necessidade do utilizador.

##  Perfil 2 — Vereadora do Urbanismo, Câmara Municipal de Lisboa

**Necessidades Principais**

4.  **Dashboards executivos** com identificação de elementos para regularização  
5.  **Alertas para anomalias**
6.  **Mapeamento por zonas** da cidade

**Implicações para a interface proposta**

- No Dashboard de Visão Geral, são apresentados indicadores-chave (KPIs) de leitura rápida. As listagens exibem alertas que podem ser filtradas para identificar elementos que requerem regularização.

- É possível visualizar alertas de anomalias em vários pontos do sistema — nas listagens, no mapa e em painéis de detalhe.

- O mapa interativo permite ao utilizador controlar o tipo de visualização e de informação apresentada, facilitando a análise de zonas específicas da cidade.

- As zonas que necessitam de regularização são destacadas através de labels de alerta na tabela associada ao mapa. No próprio mapa é possível ativar um destaque de propriedades com alertas, permitindo uma identificação imediata. 

 ##  Perfil 3 — Estudante de Mestrado em Sociologia, Universidade do Minho

 **Necessidades Principais**

7.  **Gráficos simples e impactantes**, de partilha fácil
8.  **Dados comparativos**  
9.  **Exemplos de casos emblemáticos** 

**Implicações para a interface proposta**

- Os gráficos foram concebidos com foco na simplicidade e clareza, incluindo botões de partilha direta que facilitam a disseminação em redes sociais.

- Foram criados cartões de informação otimizados para partilha, especialmente com dados gerais sobre cidades e regiões.

- Implementou-se uma frame de comparação de dados, que permite ao utilizador comparar cidades, zonas ou tipos de propriedade, apresentando resultados em diferentes níveis de detalhe.

- Para ilustrar casos emblemáticos, foram incluídas tabelas como “Top 5 Propriedades” na frame de Visão Geral e secções dedicadas a Hotspots zonas com maior densidade de alojamentos.
    
---

##  Consideração das Heurísticas de Nielsen

A seguir, apresenta-se uma análise com exemplos de como as **10 Heurísticas de Usabilidade de Jakob Nielsen** foram tidas em consideração no protótipo.

### 1. Visibilidade do estado do sistema

O sistema mantém o utilizador sempre informado sobre as ações em curso.
Por exemplo, é apresentada uma mensagem de sucesso quando são descarregados ficheiros de dados ou relatórios, garantindo que o utilizador saiba que a operação foi concluída com sucesso.

### 2. Correspondência entre o sistema e o mundo real

O sistema utiliza linguagem e ícones familiares, como o sinal de perigo para situações de alerta ou o símbolo do Euro para questões relacionadas a preços, próximos da forma como o utilizador compreende o mundo real e que ajudam a perceber o contexto. Os gráficos e mapas seguem convenções familiares (verde = boa performance, vermelho = perigo). Os termos usados são claros, evitando jargão técnico e garantindo que a linguagem é simples e compreensível por todos os utilizadores e a estrutura da informação segue uma lógica natural, alinhada com as expectativas do utilizador.

### 3. Controlo e liberdade do utilizador

O utilizador tem total controlo sobre a navegação e as suas ações, sabendo sempre onde está.
A página em que se encontra está sempre destacada no menu, permitindo uma orientação clara.
Além disso, é possível cancelar operações facilmente, como limpar todos os filtros aplicados com um único clique e tem sempre a possibilidade de voltar ao menu principal a partir de qualquer página clicando no botão que está constantemente no canto superior esquerdo.

### 4. Consistência e normas

Foi mantido um formato consistente em todas as páginas, com cabeçalho e rodapé uniformes.
Elementos que apresentam o mesmo tipo de informação seguem um padrão visual comum, e mesmo entre páginas distintas há coerência na estrutura e nos componentes, reforçando a familiaridade e reduzindo a curva de aprendizagem. Todos os botões principais têm a mesma cor e forma arredondada, o cabeçalho é constante em todas as frames e o mesmo tipo de gráfico (linhas, barras) é usado para representar o mesmo tipo de dado em diferentes páginas.

### 5. Prevenção de erros

Foram implementadas medidas preventivas para minimizar erros de utilização.
Destaca-se a técnica de ação primária dominante nos botões, como “Aplicar” e “Limpar filtros”, garantindo clareza sobre a ação principal e evitando cliques acidentais.

### 6. Reconhecimento em vez de memorização

A interface foi desenhada para reduzir o esforço de memória do utilizador.
Foram incluídos menus dropdown com opções pré-definidas (tipos de propriedade: “Casa inteira”, “Quarto privado”, “Quarto partilhado”) e funcionalidade de autocomplete na barra de pesquisa, permitindo que o utilizador reconheça opções em vez de as recordar.

### 7. Flexibilidade e eficiência de utilização

O sistema adapta-se a diferentes perfis de utilizador.
Utilizadores experientes podem descarregar relatórios personalizados de forma direta, selecionando apenas as informações desejadas, o que aumenta a eficiência e personalização da experiência.

### 8. Design estético e minimalista

O design privilegia a simplicidade e clareza, evitando elementos desnecessários que possam distrair o utilizador.
A hierarquia visual é bem definida, com uso equilibrado de cores neutras, espaços e tipografia, garantindo uma navegação fluida e agradável. Os gráficos são claros e fáceis de perceber, com espaçamente generoso e ênfase nos dados, e não nos elementos decorativos. 

### 9. Ajuda os utilizadores a reconhecer, diagnosticar e corrigir erros

As mensagens de erro são claras e construtivas, explicando o que ocorreu e sugerindo como resolver o problema.
Por exemplo,  o sistema indica se a importação de um ficheiro falhar e orienta o utilizador sobre como proceder.

### 10. Ajuda e documentação

Está disponível um botão de ajuda acessível em qualquer momento, representado por um icon intuitivo, permitindo que o utilizador consulte instruções e esclareça dúvidas rapidamente.

---

## Recomendações Futuras 

Com base na análise heurística e nos objetivos da plataforma InsideAirbnb, identificam-se várias oportunidades de melhoria e expansão para fases futuras do projeto:

### Personalização de Dashboards  
Permitir que cada utilizador (investigador, gestora pública, ativista) configure o seu painel com as métricas e visualizações mais relevantes para o seu perfil.

### Modo de Comparação Avançado  
Implementar comparações entre múltiplas cidades ou bairros, com sincronização automática das escalas nos gráficos para facilitar a leitura.

###  Melhorias de Acessibilidade  
Garantir compatibilidade com leitores de ecrã, contraste de cores adequado e navegação por teclado para utilizadores com necessidades especiais.

### Sistema de Alertas Automatizados  
Notificações automáticas sobre anomalias (aumento súbito de preços, ocupação acima de 300 dias/ano), personalizáveis por cidade ou período.

### Análise Preditiva   
Integrar modelos simples de previsão (evolução esperada de preços ou ocupação) para apoiar decisões de planeamento urbano.

---

# Conclusão 
O protótipo InsideAirbnb cumpre as principais heurísticas de usabilidade de Nielsen e responde adequadamente às necessidades dos três perfis definidos.  
O design apresenta uma estrutura consistente, linguagem clara e mecanismos de feedback visuais que favorecem a exploração e a análise de dados.  
As melhorias sugeridas concentram-se em acessibilidade, eficiência e personalização, preparando o caminho para uma implementação bem sucedida em Vue.js na segunda fase do projeto. 
