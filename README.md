# 🏭 Dashboard de Monitoramento de Perdas Industriais

## 📌 Sobre o Projeto
Na rotina de uma indústria (ex: setor de alimentos, laticínios, frigoríficos), monitorar a perda de matéria-prima é vital para proteger a margem de lucro. Este projeto é um estudo de caso focado em transformar milhares de registros operacionais em um painel executivo automatizado e claro.

O objetivo foi sair da análise linha a linha e criar um **Dashboard Interativo** que permita à diretoria tomar decisões rápidas e baseadas em dados atualizados.

## 🛠️ Tecnologias e Funções Utilizadas
- **Microsoft Excel Avançado**
- **Lógica Condicional:** Função `SE()` para criação de alertas de negócio.
- **Modelagem Relacional:** Função `PROCX()` para cruzamento seguro de tabelas dimensão e fato.
- **Estatística Descritiva com DAX:** Utilização do *Power Pivot / Modelo de Dados* para cálculos complexos (como Mediana) dentro de Tabelas Dinâmicas.

## 🚀 Desafios Resolvidos

1. **Automação de Regra de Negócio:** Criação de uma coluna de "Status" que identifica automaticamente se um lote teve perda superior a 5% do peso esperado, emitindo um "Alerta de Perda".
2. **Cruzamento de Informações:** Desenvolvimento de uma estrutura relacional (simulando chaves de Banco de Dados) para buscar automaticamente os supervisores de cada setor, tornando a planilha imune a erros de digitação e escalável para novos setores.
3. **Visão Executiva (Pivot Table):** Criação de um resumo gerencial interativo.

## 💡 Insights de Negócio e Estatística

Em linhas de produção, utilizar apenas a **Média** para medir perdas pode mascarar a realidade, já que um único erro grave de maquinário (*outlier*) joga a média para cima. 

Neste painel, implementamos o cálculo da **Mediana** utilizando a linguagem DAX. A Mediana isola essas falhas pontuais e revela o comportamento padrão diário do chão de fábrica, permitindo ao gestor focar no problema real sem pânico desnecessário. O uso de segmentação de dados (filtros por Status e Supervisor) transforma a tabela em uma ferramenta de investigação de gargalos.

## 📂 Como navegar neste repositório
- `cortes_perdas_usando_excel.xlsx`: Arquivo original com a base de dados, modelagem e a Tabela Dinâmica final.
- `Insights Base Excel.pdf`: Documento executivo detalhando o passo a passo da solução com imagens.
- `img_excel_01.png` a `04.png`: Imagens de demonstração do projeto (utilizadas para apresentação técnica).

---
*Projeto desenvolvido como parte do portfólio de Engenharia e Análise de Dados.*
