# RefTrab - Análise das Emendas da Reforma Trabalhista

**Investigação jornalística que revelou a autoria real das emendas da Reforma Trabalhista de 2017 através de análise de metadados de PDFs**

## 📰 Sobre o Projeto

Este repositório contém o código e metodologia utilizados pelo jornalista **Reinaldo Chaves** para a reportagem investigativa do **The Intercept Brasil** intitulada ["Lobistas de bancos, indústrias e transportes estão por trás das emendas da Reforma Trabalhista"](https://www.intercept.com.br/2017/04/26/lobistas-de-bancos-industrias-e-transportes-quem-esta-por-tras-das-emendas-da-reforma-trabalhista/), publicada em 26 de abril de 2017.

### 🎯 Descoberta Principal

A investigação revelou que **34,3% das 850 emendas** apresentadas por deputados à Reforma Trabalhista foram na verdade **redigidas por lobistas** de associações empresariais, incluindo:

- **Confederação Nacional do Transporte (CNT)**
- **Confederação Nacional das Instituições Financeiras (CNF)**  
- **Confederação Nacional da Indústria (CNI)**
- **Associação Nacional do Transporte de Cargas e Logística (NTC&Logística)**

## 🔍 Metodologia

### Análise de Metadados de PDFs

O projeto utilizou análise forense de metadados para identificar a autoria real dos documentos:

1. **Extração de Metadados**: Análise dos metadados dos arquivos PDF das emendas protocoladas na Câmara dos Deputados
2. **Identificação do Autor**: Verificação do campo "autor" nos metadados que indica o usuário/computador onde o arquivo foi criado
3. **Mapeamento de Origens**: Correlação entre os autores identificados e funcionários de entidades empresariais
4. **Análise de Padrões**: Identificação de emendas clonadas com textos idênticos apresentadas por diferentes deputados

### Dados Analisados

- **850 emendas** apresentadas por **82 deputados**
- **292 emendas (34,3%)** com autoria de entidades empresariais
- **113 emendas** com autoria confirmada de funcionários das 4 entidades citadas
- **52,4%** das emendas de lobistas foram incorporadas ao projeto final

## 📊 Principais Descobertas

### Deputados que Mais Apresentaram Emendas de Lobistas

- **Major Olímpio (SD-SP)**: 31 emendas (28 de entidades empresariais)
- **Diego Andrade (PSD-MG)**: 22 emendas (todas da CNT)
- **Renzo Braz (PP-MG)**: 19 emendas (todas da CNT)
- **Mauro Lopes (PMDB-MG)**: 24 emendas (CNT e NTC&Logística)

### Conflitos de Interesse Identificados

- Diego Andrade é sobrinho do presidente da CNT
- Renzo Braz tem família ligada ao transporte de cargas
- Vários deputados receberam doações de empresas dos setores beneficiados

### Outras Origens Identificadas

- **22 emendas** redigidas pelo presidente da Associação Nacional dos Procuradores do Trabalho
- **11 emendas** com autoria atribuída ao TST (Tribunal Superior do Trabalho)
- Terminal **"P_4189"** usado como "copiadora" de emendas para diferentes deputados

## 🛠️ Ferramentas e Tecnologias

O projeto utilizou:

- **Python** para análise de dados
- **Jupyter Notebook** (`chupaemenda.ipynb`)
- Bibliotecas para extração de metadados de PDFs
- Scripts de análise e correlação de dados

## 📁 Estrutura do Repositório

```
reftrab/
├── chupaemenda.ipynb     # Notebook principal com análise das emendas
├── README.md             # Este arquivo
└── [outros arquivos]     # Scripts e dados complementares
```

## 🔗 Links Importantes

- **Reportagem Original**: [The Intercept Brasil](https://www.intercept.com.br/2017/04/26/lobistas-de-bancos-industrias-e-transportes-quem-esta-por-tras-das-emendas-da-reforma-trabalhista/)
- **Lista de Deputados**: [Deputados que apresentaram emendas de lobistas](https://theintercept.com/document/2017/04/26/deputados-que-apresentaram-emendas-de-lobistas-para-reforma-trabalhista/)
- **Portal da Câmara**: [PL 6787/2016 - Reforma Trabalhista](https://www.camara.leg.br/proposicoesWeb/fichadetramitacao?idProposicao=2122076)

## 🎖️ Impacto e Reconhecimento

Esta investigação:

- Revelou esquema de lobby não transparente no Congresso Nacional
- Demonstrou conflitos de interesse na elaboração de legislação
- Contribuiu para o debate sobre regulamentação do lobby no Brasil
- Exemplificou o uso de jornalismo de dados para investigações de interesse público

## 👥 Equipe da Reportagem

**Reportagem**: Alline Magalhães, Breno Costa, Lúcio Lambranho, Reinaldo Chaves  
**Colaboração**: Bruno Pavan, Jéssica Sbardelotto, Rodrigo Menegat  
**Análise de Dados**: Reinaldo Chaves

## 📧 Contato

**Reinaldo Chaves**  
- Email: reichaves@gmail.com
- LinkedIn: [reinaldochaves](https://www.linkedin.com/in/reinaldochaves/)
- GitHub: [@reichaves](https://github.com/reichaves)

## ⚖️ Contexto Legal

A investigação revelou que embora o lobby não seja crime no Brasil, a apresentação de emendas por entidades privadas através de parlamentares pode configurar:

- Violação do regimento da Câmara dos Deputados
- Possível corrupção passiva (segundo especialistas consultados)
- Conflito de interesses não declarado

## 📚 Metodologia Jornalística

Este projeto é um exemplo de:

- **Jornalismo de Dados**: Uso de análise computacional para investigação
- **Jornalismo Investigativo**: Revelação de informações de interesse público
- **Transparência Governamental**: Monitoramento da atividade legislativa
- **Accountability**: Responsabilização de agentes públicos

## 🔄 Reprodutibilidade

O código disponibilizado permite:

- Replicar a análise realizada
- Adaptar a metodologia para outras investigações
- Verificar as descobertas da reportagem
- Aplicar técnicas similares em outros contextos

---

*Este projeto representa um marco no jornalismo investigativo brasileiro, demonstrando como técnicas de análise de dados podem revelar práticas não transparentes no poder público e contribuir para o fortalecimento da democracia.*

## 📄 Licença

Este projeto está disponível para fins educacionais e de pesquisa, respeitando os direitos autorais da reportagem original do The Intercept Brasil.

---

**"Jornalista que gosta de The Who, matemática e programar"** - Reinaldo Chaves
