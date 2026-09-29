# Ficha de Avaliação de Processo (PDD) — Questão 5

> MOLDE. Copie para `entregas/SEU_RA/` e preencha. Escolha **um** cenário (A ou B).

**Cenário escolhido:** <A>

1. **Nome do processo e descrição resumida:**
   <Processamento e Lançamento de Notas Fiscais de Entrada (Contas a Pagar). O processo consiste em monitorar uma caixa de e-mails corporativa onde chegam notas fiscais em formato PDF ou XML, extrair automaticamente os dados chave (número da nota, CNPJ, valor e vencimento) e realizar o cadastro/lançamento dessas informações no sistema ERP da empresa.>

2. **Volume / frequência estimados:**
   <Cerca de 300 a 500 notas fiscais por dia, com recebimento contínuo durante o horário comercial e picos no fechamento de mês.>

3. **As entradas são estruturadas?** (sim/não + justificativa)
   <Sim. As informações chegam em arquivos digitais padronizados (XMLs estruturados ou PDFs com layout fixo), contendo campos bem definidos (como valor, CNPJ e data), o que facilita a leitura automatizada por softwares de OCR ou parsers de texto.>

4. **As regras são claras e determinísticas?** (sim/não + justificativa)
   <Sim. O fluxo segue um conjunto rígido de regras lógicas: se o CNPJ do fornecedor for válido e o valor corresponder ao pedido de compra, o robô aprova e cadastra no ERP; caso contrário, a nota é direcionada para uma exceção humana. Não há margem para julgamento subjetivo ou interpretação pessoal.>

5. **Veredito — o processo é elegível a RPA?** (justifique com base em regras
   claras, dados estruturados e repetibilidade)
   <Sim, o processo é altamente elegível a RPA. Justificativa: Trata-se de uma tarefa repetitiva, de alto volume diário, baseada em regras estritamente determinísticas, utilizando dados digitais estruturados e exigindo movimentação entre sistemas (e-mail, leitor de arquivos e ERP). A automação eliminará o erro humano, reduzirá o tempo de processamento e liberará a equipe fiscal para tarefas analíticas.>
