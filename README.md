# Relatórios Power BI

Coleção de relatórios desenvolvidos no Microsoft Power BI para análise de dados financeiros e gestão de vendas. Dashboards interativos com visualizações estratégicas para tomada de decisão.

[Relatórios](#relatórios-disponíveis) • [Funcionalidades](#funcionalidades) • [Instalação](#instalação) • [Uso](#uso)

## Índice

- Sobre o Projeto
- Relatórios Disponíveis
- Funcionalidades
- Instalação
- Uso
- Estrutura dos Dados
- Contribuindo

## Sobre o Projeto

Este repositório contém dois relatórios completos desenvolvidos no Microsoft Power BI, focados em análise financeira e gestão comercial. Os dashboards oferecem visualizações interativas, filtros dinâmicos e métricas estratégicas para apoio à tomada de decisão empresarial.

### Principais Características

- **Visualizações Interativas** - Gráficos e tabelas dinâmicas para exploração de dados
- **Análise Temporal** - Comparativos e tendências ao longo do tempo
- **Filtros Avançados** - Segmentação por múltiplas dimensões de negócio
- **KPIs Estratégicos** - Indicadores chave de performance em tempo real
- **Design Responsivo** - Interface otimizada para diferentes dispositivos
- **Exportação de Dados** - Relatórios exportáveis em diversos formatos

## Relatórios Disponíveis

### 1. Sample Financial (`sample_financial.pbix`)

Dashboard completo de análise financeira com métricas e indicadores estratégicos.

#### Funcionalidades

- Visualização de performance financeira consolidada
- Análise de receitas, custos e margens
- Comparativos históricos e projeções
- Segmentação por período, produto ou região
- Indicadores de rentabilidade e eficiência

**Uso recomendado**: Análise financeira, acompanhamento de resultados, apresentações executivas e planejamento estratégico.

### 2. Gestão de Vendas (`gestaoVendas.pbix`)

Dashboard focado em performance comercial e análise de vendas.

#### Funcionalidades

- Acompanhamento de volumes e receitas de vendas
- Análise de desempenho por vendedor, produto ou cliente
- Métricas de conversão e ticket médio
- Tendências de vendas e sazonalidade
- Identificação de oportunidades e gargalos

**Uso recomendado**: Gestão comercial, análise de performance de vendas, planejamento de metas e estratégias de crescimento.

## Funcionalidades

### Análise de Dados

- ✅ Visualizações gráficas interativas (linhas, barras, pizza, etc.)
- ✅ Tabelas dinâmicas com drill-down
- ✅ Filtros e segmentadores customizáveis
- ✅ Cálculos e medidas personalizadas (DAX)
- ✅ Relacionamentos entre múltiplas tabelas

### Interatividade

- ✅ Cross-filtering entre visualizações
- ✅ Tooltips personalizados com informações detalhadas
- ✅ Bookmarks para salvar visualizações específicas
- ✅ Navegação entre páginas do relatório
- ✅ Exportação para PDF, PowerPoint e Excel

### Performance

- ✅ Otimização de consultas e modelos de dados
- ✅ Carga incremental de dados
- ✅ Compressão de dados para melhor desempenho
- ✅ Cache de consultas para acesso rápido

## Instalação

### Pré-requisitos

- **Power BI Desktop** - [Download](https://powerbi.microsoft.com/pt-br/desktop/)
- **Windows 10/11** - Sistema operacional compatível
- **4GB RAM** - Mínimo recomendado (8GB+ ideal)

### Instalação com Power BI Desktop

#### 1. Clone o repositório

```bash
git clone https://github.com/nevesmarcos42/PowerBI.git
cd PowerBI
```

#### 2. Abra o relatório

1. Localize o arquivo `.pbix` desejado
2. Dê um duplo clique no arquivo
3. O Power BI Desktop será iniciado automaticamente
4. Aguarde o carregamento dos dados

#### 3. Atualize as fontes de dados (se necessário)

```
1. Vá em "Página Inicial" > "Transformar Dados" > "Configurações da Fonte de Dados"
2. Atualize as credenciais e caminhos das fontes
3. Clique em "Atualizar" para carregar os dados mais recentes
```

## Uso

### Primeiro Acesso

1. **Abra o relatório**: Dê um duplo clique no arquivo `.pbix` desejado
2. **Navegue pelas páginas**: Use as guias na parte inferior para alternar entre dashboards
3. **Interaja com os filtros**: Clique nos segmentadores para filtrar os dados
4. **Explore visualizações**: Clique em elementos dos gráficos para fazer drill-down

### Funcionalidades Principais

#### Filtrar Dados

1. Use os segmentadores (slicers) disponíveis em cada página
2. Clique em elementos de gráficos para filtrar cruzado
3. Use o painel de filtros à direita para filtros avançados

#### Atualizar Dados

```
1. Clique em "Página Inicial" > "Atualizar"
2. Aguarde a atualização das fontes de dados
3. Verifique a data/hora da última atualização no canto do relatório
```

#### Exportar Relatórios

```
1. Vá em "Arquivo" > "Exportar"
2. Escolha o formato desejado (PDF, PowerPoint, etc.)
3. Configure as opções de exportação
4. Salve o arquivo no local desejado
```

#### Publicar no Power BI Service

```
1. Clique em "Página Inicial" > "Publicar"
2. Selecione o workspace de destino
3. Configure as permissões de acesso
4. Compartilhe o link com sua equipe
```

## Estrutura dos Dados

### Sample Financial

```
Tabelas:
├── Financials          # Dados financeiros consolidados
│   ├── Date            # Datas das transações
│   ├── Product         # Produtos/serviços
│   ├── Segment         # Segmentos de mercado
│   ├── Country         # Países/regiões
│   ├── Units Sold      # Unidades vendidas
│   ├── Revenue         # Receita
│   ├── Profit          # Lucro
│   └── COGS            # Custo dos produtos vendidos

Medidas:
├── Total Revenue       # Receita total
├── Total Profit        # Lucro total
├── Profit Margin       # Margem de lucro
└── YoY Growth          # Crescimento ano a ano
```

### Gestão de Vendas

```
Tabelas:
├── Sales               # Dados de vendas
│   ├── Date            # Data da venda
│   ├── Product         # Produto vendido
│   ├── Customer        # Cliente
│   ├── Salesperson     # Vendedor
│   ├── Quantity        # Quantidade
│   ├── Unit Price      # Preço unitário
│   └── Total Amount    # Valor total

Medidas:
├── Total Sales         # Vendas totais
├── Average Ticket      # Ticket médio
├── Conversion Rate     # Taxa de conversão
└── Sales Growth        # Crescimento de vendas
```

## Formato dos Arquivos

| Item                | Descrição                             |
| ------------------- | ------------------------------------- |
| **Extensão**        | `.pbix` (Power BI Desktop File)       |
| **Plataforma**      | Microsoft Power BI                    |
| **Compatibilidade** | Power BI Desktop e Power BI Service   |
| **Tamanho**         | Variável (depende do volume de dados) |

## Atualizações

### Atualização Manual

1. Abra o arquivo no Power BI Desktop
2. Clique em "Atualizar" na barra de ferramentas
3. Aguarde a sincronização com as fontes de dados

### Atualização Automática (Power BI Service)

1. Publique o relatório no Power BI Service
2. Configure um gateway de dados (se necessário)
3. Agende atualizações automáticas nas configurações do dataset
4. Defina frequência e horários de atualização

## Observações

- Os relatórios podem conter conexões com fontes de dados específicas
- Certifique-se de ter as permissões adequadas para acessar as fontes de dados
- Alguns recursos podem requerer licença do Power BI Pro ou Premium
- Para compartilhamento online, é necessário publicar no Power BI Service
- Recomenda-se backup regular dos arquivos `.pbix`

## Contribuindo

Contribuições são bem-vindas! Siga os passos:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

### Padrões de Desenvolvimento

#### Power BI

- Seguir convenções de nomenclatura para medidas e colunas
- Documentar fórmulas DAX complexas
- Otimizar relacionamentos entre tabelas
- Manter modelo de dados normalizado
- Adicionar tooltips explicativos nas visualizações

#### Dados

- Validar integridade dos dados antes de publicar
- Remover colunas e tabelas não utilizadas
- Usar tipos de dados apropriados
- Documentar transformações realizadas no Power Query

---

**Versão**: 1.0.0

**Última atualização**: Novembro 2025

Desenvolvido como projeto de análise de dados com Power BI
