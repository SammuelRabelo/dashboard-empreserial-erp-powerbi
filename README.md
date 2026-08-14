# 📊 Dashboard de Diagnóstico e Análise de Resultados

## 📝 Sobre o Projeto
Este projeto de Business Intelligence foi desenvolvido sob demanda para um **cliente real**. O principal desafio do projeto era superar as limitações do sistema ERP utilizado pela empresa, que era engessado e não oferecia facilidade ou flexibilidade para a geração de relatórios gerenciais.

O objetivo do dashboard é atuar como a camada de inteligência da empresa: ele extrai os dados diretamente desse ERP e os transforma em visualizações claras e interativas. Com isso, o projeto democratizou o acesso à informação, auxiliando ativamente na tomada de decisão estratégica em **todas as principais áreas da empresa** (Comercial, CRM, Faturamento e Financeiro).

> **Nota:** Os dados expostos nas imagens e vídeos deste repositório foram anonimizados (substituídos por dados fictícios ou ocultados) por questões de confidencialidade e respeito à privacidade do cliente.

## 🎥 Demonstração em Vídeo
Confira abaixo a navegação, os filtros dinâmicos e as funcionalidades do dashboard em ação:


https://github.com/user-attachments/assets/d123d51a-1087-4c38-8beb-f047661d4036


## 📸 Telas do Dashboard

**1.1 Metas e KPIs:**
<img width="2050" height="1154" alt="1 1 Metas e KPIs" src="https://github.com/user-attachments/assets/9c1b0cd8-1c80-4e4f-bf19-016b1fecbb34" />


**2.1 Resumo Vendas:**
<img width="2050" height="1152" alt="2 1 Resumo Vendas" src="https://github.com/user-attachments/assets/49477086-7869-49db-8823-1cc596897125" />


**2.2 Faturamento e Nota Fiscal:**
<img width="2050" height="1148" alt="2 2 Faturamento e Nota Fiscal" src="https://github.com/user-attachments/assets/3ff4cf7a-fb15-49c6-8d4f-4541dd9bc3aa" />


**2.3 Produtos e Fabricantes:**
<img width="2054" height="1154" alt="2 3 Produtos e Fabricantes" src="https://github.com/user-attachments/assets/53622cc6-cb9f-4822-8f81-4d6798052526" />


**3.1 Pipeline:**
<img width="2052" height="1154" alt="3 1 Pipeline" src="https://github.com/user-attachments/assets/87eefa9b-5e90-454f-a961-ca81c5b0d48e" />


**3.2 Clientes:**
<img width="2054" height="1154" alt="3 2 Clientes" src="https://github.com/user-attachments/assets/61318eb0-c4ac-4e02-83d5-ef43accb5b1a" />


**3.3 Visitas e Telemarketing:**
<img width="2046" height="1152" alt="3 3 Visitas e Telemarketing" src="https://github.com/user-attachments/assets/dfa46103-4860-4935-9c05-f2bfdad5455e" />


**3.4 Vendedores:**
<img width="2050" height="1156" alt="3 4 Vendedores" src="https://github.com/user-attachments/assets/398e3337-04f3-44f9-bbca-b6a5fee9beba" />


**4.1 Contas a Receber:**
<img width="2050" height="1152" alt="4 1 Contas a Receber" src="https://github.com/user-attachments/assets/229caa16-5289-4780-9227-5958d54f228f" />


**4.2 Contas a Pagar:**
<img width="2052" height="1150" alt="4 2 Contas a Pagar" src="https://github.com/user-attachments/assets/f592b536-ba3a-4002-b3df-c1cd725570d2" />


**4.3 Resumo Financeiro:**
<img width="2050" height="1156" alt="4 3 Resumo Financeiro" src="https://github.com/user-attachments/assets/2506dee8-3bca-4f38-9890-b88288e7401e" />


**4.4 DRE:**
<img width="2050" height="1158" alt="4 4 DRE" src="https://github.com/user-attachments/assets/9f2cf19e-d08e-490e-9e6c-8abe17528b85" />


**4.5 Folha Salarial:**
<img width="2050" height="1162" alt="4 5 Folha de Pagamento" src="https://github.com/user-attachments/assets/fa4332e3-4377-47f1-bd44-5aa8c8a82e0b" />


**5.1 Estoque:**
<img width="2046" height="1158" alt="5 1 Estoque" src="https://github.com/user-attachments/assets/82e497de-e627-43f8-87e3-cd9222171521" />


---

## 🏗️ 1. Arquitetura do Modelo de Dados

O modelo foi construído utilizando os princípios de **Star Schema** para otimização de performance no Power BI. O projeto contempla múltiplas visões de negócio: **Financeiro** (Contas a Pagar/Receber, DRE) e **CRM/Comercial** (Propostas, Visitas, Vendas, Metas).

### 📐 Tabelas Fato (Transacionais)
As tabelas fato contêm os eventos de negócio e métricas quantitativas.
- **`Dias Inatividade`** (1 colunas)
- **`sgr_conta_pagar_Consolidada
`** (32 colunas)
- **`sgr_conta_receber_Consolidada
`** (33 colunas)
- **`vw_Cliente_NotaFiscal_BI_Consolidada
`** (20 colunas)
- **`vw_Clientes_Pbi_Consolidada
`** (12 colunas)
- **`vw_Comissoes_Pbi_Consolidada
`** (7 colunas)
- **`vw_Conversao_Unidade_Pbi_Consolidada
`** (3 colunas)
- **`vw_DRE_Receita_Deducoes_Pbi_Consolidada
`** (4 colunas)
- **`vw_Estoque_Lote_Pbi_Consolidada
`** (9 colunas)
- **`vw_Fornecedores_Pbi_Consolidada
`** (7 colunas)
- **`vw_Lancamentos_DRE_Pbi_Conslidada
`** (13 colunas)
- **`vw_Metas_Pbi_Consolidada
`** (17 colunas)
- **`vw_Orcamento_Compra_Pbi_Consolidada
`** (11 colunas)
- **`vw_Pedidos_Pbi_Consolidada
`** (18 colunas)
- **`vw_Plano_Contas_Pbi_Consolidada
`** (17 colunas)
- **`vw_Produtos_Pbi_Consolidada
`** (17 colunas)
- **`vw_Propostas_Pbi_Consolidada
`** (12 colunas)
- **`vw_Vendedores_Pbi_Consolidada
`** (3 colunas)
- **`vw_Visitas_Pbi_Consolidada
`** (16 colunas)
- **`vw_telemarketing_Pbi_Consolidada
`** (14 colunas)

### 🏷️ Tabelas Dimensão (Cadastros e Filtros)
- **`dCalendario
`** (14 colunas)
- **`dDRE_Completo
`** (6 colunas)
- **`dEmpresa
`** (1 colunas)
- **`dLinhasDRE
`** (3 colunas)
- **`dMultiplicadorImportacao
`** (3 colunas)
- **`dPlanoContas_Pagar
`** (1 colunas)
- **`dPlanoContas_Receber
`** (1 colunas)
- **`dStatusParcela
`** (2 colunas)

---

## 🔗 2. Relacionamentos do Modelo
As tabelas estão conectadas garantindo o fluxo de filtros correto (propagações unidirecionais em sua maioria). Abaixo, as principais conexões:

- `vw_Cliente_NotaFiscal_BI_Consolidada.Empresa -> dEmpresa.Empresa`
- `vw_Propostas_Pbi_Consolidada.Empresa -> dEmpresa.Empresa`
- `sgr_conta_receber_Consolidada.Empresa -> dEmpresa.Empresa`
- `sgr_conta_pagar_Consolidada.Empresa -> dEmpresa.Empresa`
- `sgr_conta_pagar_Consolidada.Plano_Contas_Debito -> dPlanoContas_Pagar.Plano_Contas`
- `sgr_conta_receber_Consolidada.Plano_Contas_Credito -> dPlanoContas_Receber.Plano_Contas`
- `vw_Estoque_Lote_Pbi_Consolidada.Empresa -> dEmpresa.Empresa`
- `vw_Cliente_NotaFiscal_BI_Consolidada.Codigo_Cliente -> vw_Clientes_Pbi_Consolidada.Codigo_Cliente`
- `vw_Cliente_NotaFiscal_BI_Consolidada.Codigo_Produto -> vw_Produtos_Pbi_Consolidada.Codigo_Produto`
- `vw_Cliente_NotaFiscal_BI_Consolidada.Codigo_Fornecedor -> vw_Fornecedores_Pbi_Consolidada.Codigo_Fornecedor`
- `vw_Cliente_NotaFiscal_BI_Consolidada.Codigo_Vendedor -> vw_Vendedores_Pbi_Consolidada.Codigo_Vendedor`
- `vw_Propostas_Pbi_Consolidada.Codigo_Cliente -> vw_Clientes_Pbi_Consolidada.Codigo_Cliente`
- `vw_Propostas_Pbi_Consolidada.Codigo_Vendedor -> vw_Vendedores_Pbi_Consolidada.Codigo_Vendedor`
- `sgr_conta_receber_Consolidada.Codigo_Cliente -> vw_Clientes_Pbi_Consolidada.Codigo_Cliente`
- `sgr_conta_pagar_Consolidada.Codigo_Cliente -> vw_Fornecedores_Pbi_Consolidada.Codigo_Fornecedor`
- *(e outros relacionamentos estruturais...)*

---

## 🧮 3. Dicionário de Medidas DAX

O projeto contém dezenas de cálculos dinâmicos agrupados em tabelas de medidas. Abaixo estão listadas algumas das fórmulas mais relevantes.

### 💰 Financeiro (Amostra de Medidas)

**Total a Receber**
```dax
SUM(sgr_conta_receber_Consolidada[Valor_Parcela])
```

**Receber em Aberto**
```dax
CALCULATE(
			    SUM(sgr_conta_receber_Consolidada[Valor_Parcela]),
			    ISBLANK(sgr_conta_receber_Consolidada[Data_Quitacao])
			)
```

**Total Recebido**
```dax
CALCULATE(
			    SUM(sgr_conta_receber_Consolidada[Valor_Parcela]),
			    NOT ISBLANK(sgr_conta_receber_Consolidada[Data_Quitacao])
			)
```

**Receber Vencido**
```dax
CALCULATE(
			    SUM(sgr_conta_receber_Consolidada[Valor_Parcela]),
			    sgr_conta_receber_Consolidada[Faixa Aging] IN {"1-7 dias", "8-15 dias", "16-30 dias", "31-60 dias", "61-90 dias", "+90 dias"}
			)
```

**% Inadimplencia**
```dax
DIVIDE([Receber Vencido], [Receber em Aberto])
```

**DSO Prazo Medio Recebimento**
```dax
VAR _Pagas =
			    FILTER(
			        sgr_conta_receber_Consolidada,
			        NOT ISBLANK(sgr_conta_receber_Consolidada[Data_Quitacao])
			    )
			RETURN
			    AVERAGEX(
			        _Pagas,
			        INT(sgr_conta_receber_Consolidada[Data_Quitacao] - sgr_conta_receber_Consolidada[Data_Emissao])
			    )
```

**Recebido Mes Anterior**
```dax
CALCULATE([Total Recebido], PREVIOUSMONTH(dCalendario[Date]))
```

**Total a Pagar**
```dax
SUM(sgr_conta_pagar_Consolidada[Valor_Parcela])
```

**Pagar em Aberto**
```dax
CALCULATE(
			    SUM(sgr_conta_pagar_Consolidada[Valor_Parcela]),
			    ISBLANK(sgr_conta_pagar_Consolidada[Data_Quitacao])
			)
```

**Total Pago**
```dax
CALCULATE(
			    SUM(sgr_conta_pagar_Consolidada[Valor_Parcela]),
			    NOT ISBLANK(sgr_conta_pagar_Consolidada[Data_Quitacao])
			)
```

**Pagar Vencido**
```dax
CALCULATE(
			    SUM(sgr_conta_pagar_Consolidada[Valor_Parcela]),
			    sgr_conta_pagar_Consolidada[Faixa Aging] IN {"1-7 dias", "8-15 dias", "16-30 dias", "31-60 dias", "61-90 dias", "+90 dias"}
			)
```

**Pagar a Vencer**
```dax
CALCULATE(
			    SUM(sgr_conta_pagar_Consolidada[Valor_Parcela]),
			    sgr_conta_pagar_Consolidada[Faixa Aging] IN {"A vencer", "Vence hoje"}
			)
```

**DPO Prazo Medio Pagamento**
```dax
VAR _Pagas =
			    FILTER(
			        sgr_conta_pagar_Consolidada,
			        NOT ISBLANK(sgr_conta_pagar_Consolidada[Data_Quitacao])
			    )
			RETURN
			    AVERAGEX(
			        _Pagas,
			        INT(sgr_conta_pagar_Consolidada[Data_Quitacao] - sgr_conta_pagar_Consolidada[Data_Emissao])
			    )
```

**Pago Mes Anterior**
```dax
CALCULATE([Total Pago], PREVIOUSMONTH(dCalendario[Date]))
```

**Saldo do Periodo**
```dax
[Total Recebido] - [Total Pago]
```

### 🤝 CRM e Comercial (Amostra de Medidas)

**Faturamento Total**
```dax
VAR _NotasUnicas =
			    CALCULATETABLE(
			        SUMMARIZE(
			            vw_Cliente_NotaFiscal_BI_Consolidada,
			            vw_Cliente_NotaFiscal_BI_Consolidada[Empresa],
			            vw_Cliente_NotaFiscal_BI_Consolidada[Numero_Nota],
			            vw_Cliente_NotaFiscal_BI_Consolidada[Valor_Total_Nota]
			        ),
			        vw_Cliente_NotaFiscal_BI_Consolidada[Situacao_Nota] = "Transmitida",
			        vw_Cliente_NotaFiscal_BI_Consolidada[Tipo_de_Nota_Fiscal] = "VENDA"
			    )
			RETURN
			    SUMX(_NotasUnicas, vw_Cliente_NotaFiscal_BI_Consolidada[Valor_Total_Nota])
```

**Qtd de Notas Emitidas**
```dax
CALCULATE(
			    DISTINCTCOUNT(vw_Cliente_NotaFiscal_BI_Consolidada[Numero_Nota]),
			    vw_Cliente_NotaFiscal_BI_Consolidada[Situacao_Nota] = "Transmitida",
			    vw_Cliente_NotaFiscal_BI_Consolidada[Tipo_de_Nota_Fiscal] = "VENDA"
			)
```

**Total de Propostas**
```dax
DISTINCTCOUNT(vw_Propostas_Pbi_Consolidada[Codigo_Proposta])
```

**Propostas Fechadas**
```dax
CALCULATE(
			    DISTINCTCOUNT(vw_Propostas_Pbi_Consolidada[Codigo_Proposta]),
			    vw_Propostas_Pbi_Consolidada[Status_Situacao] = "Fechado"
			)
```

**Propostas Em Andamento**
```dax
CALCULATE(
			    DISTINCTCOUNT(vw_Propostas_Pbi_Consolidada[Codigo_Proposta]),
			    vw_Propostas_Pbi_Consolidada[Status_Situacao] = "Em Andamento"
			)
```

**Propostas Perdidas**
```dax
CALCULATE(
			    DISTINCTCOUNT(vw_Propostas_Pbi_Consolidada[Codigo_Proposta]),
			    vw_Propostas_Pbi_Consolidada[Status_Situacao] = "Perdido"
			)
```

**Taxa de Conversao %**
```dax
DIVIDE(
			    [Propostas Fechadas],
			    [Propostas Fechadas] + [Propostas Perdidas]
			)
```

**Valor do Pipeline**
```dax
SUMX(
			    FILTER(
			        SUMMARIZE(
			            vw_Propostas_Pbi_Consolidada,
			            vw_Propostas_Pbi_Consolidada[Codigo_Proposta],
			            vw_Propostas_Pbi_Consolidada[Status_Situacao],
			            vw_Propostas_Pbi_Consolidada[Valor_Total_Proposta]
			        ),
			        vw_Propostas_Pbi_Consolidada[Status_Situacao] = "Em Andamento"
			    ),
			    vw_Propostas_Pbi_Consolidada[Valor_Total_Proposta]
			)
```

**Clientes Ativos**
```dax
CALCULATE(
			    DISTINCTCOUNT(vw_Cliente_NotaFiscal_BI_Consolidada[Codigo_Cliente]),
			    vw_Cliente_NotaFiscal_BI_Consolidada[Situacao_Nota] = "Transmitida",
			    vw_Cliente_NotaFiscal_BI_Consolidada[Tipo_de_Nota_Fiscal] = "VENDA"
			)
```

**Total de Clientes Cadastrados**
```dax
COUNTROWS(vw_Clientes_Pbi_Consolidada)
```

**Clientes Sem Compra**
```dax
[Total de Clientes Cadastrados] - [Clientes Ativos]
```

**Novos Clientes**
```dax
CALCULATE(
			    COUNTROWS(vw_Clientes_Pbi_Consolidada),
			    USERELATIONSHIP(vw_Clientes_Pbi_Consolidada[Data_Cadastro_Cliente], dCalendario[Date])
			)
```

**Faturamento por Cliente**
```dax
DIVIDE([Faturamento Total], [Clientes Ativos])
```

**Concentracao Top 5 %**
```dax
VAR _Top5 =
			    TOPN(
			        5,
			        VALUES(vw_Clientes_Pbi_Consolidada[Codigo_Cliente]),
			        [Faturamento Total], DESC
			    )
			VAR _FatTop5 =
			    CALCULATE([Faturamento Total], KEEPFILTERS(_Top5))
			RETURN
			    DIVIDE(_FatTop5, [Faturamento Total])
```

**Faturamento por Vendedor**
```dax
CALCULATE(
			    [Faturamento Total],
			    VALUES(vw_Cliente_NotaFiscal_BI_Consolidada[Nome_Vendedor])
			)
```

---
