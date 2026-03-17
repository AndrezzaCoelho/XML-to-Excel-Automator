RoboNotas: Extrator e Automatizador de XML Fiscal 📊
O RoboNotas é uma ferramenta desenvolvida em Python para automatizar a leitura de arquivos XML de Notas Fiscais de Serviço (NFS-e) e a geração de relatórios detalhados em Excel. O projeto foi idealizado para otimizar processos contábeis, eliminando a digitação manual e garantindo a integridade dos dados fiscais.

 Funcionalidades
Extração Inteligente: Identifica automaticamente tags de CNPJ, Razão Social e valores de impostos em diferentes formatos de XML.

Cálculos Automáticos: Realiza o cálculo de Retenções Federais e do Valor Líquido das notas processadas.

Identificação de Status: Detecta automaticamente se uma nota está "Ativa" ou "Cancelada" com base nas tags do arquivo.

Interface Gráfica (GUI): Utiliza o Tkinter para que o usuário selecione a pasta de arquivos de forma simples e intuitiva.

Relatórios Formatados: Gera um arquivo .xlsx com formatação condicional, cabeçalhos destacados e colunas financeiras configuradas para moeda (R$).

 Tecnologias Utilizadas
Python 3: Linguagem base do projeto.

Pandas: Manipulação e estruturação dos dados em DataFrames.

ElementTree (ET): Parsing e navegação na estrutura dos arquivos XML.

XlsxWriter: Engine para criação e formatação avançada de arquivos Excel.

Tkinter: Interface para seleção de diretórios e exibição de mensagens.

 Como Executar
Instale as dependências necessárias:

Bash
pip install pandas xlsxwriter
(Nota: No Linux, pode ser necessário instalar o suporte ao Tkinter via sudo apt install python3-tk).

Execute o script:

Bash
python "robo_notas 2.py"
Selecione a pasta: Uma janela será aberta para você escolher o diretório onde os arquivos XML estão armazenados. O relatório será salvo automaticamente na mesma pasta com o nome Relatorio_Notas.xlsx.

 Campos Extraídos
O robô coleta e organiza as seguintes informações:

Status da Nota, Número (NFS-e) e Data de Emissão.

Dados do Prestador e Tomador (CNPJ e Razão Social).

Impostos: PIS/PASEP, COFINS, CSLL, INSS, IRPJ e ISS.

Descrição do Serviço e Código NBS.

Desenvolvido por Andrezza Coelho como parte de projetos de automação para o setor de tecnologia e contabilidade.
