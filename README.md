Relatório DeskManager: Automatizador de Análise de Chamados
Visão Geral
O Relatório DeskManager é um aplicativo web estático desenvolvido para otimizar a geração de relatórios mensais de atendimentos, convertendo dados brutos de planilhas exportadas do DeskManager em insights estratégicos. Ele automatiza a filtragem e o cálculo de indicadores-chave, eliminando a necessidade de processos manuais e garantindo a consistência e precisão das análises.

Objetivo
O principal objetivo do projeto é automatizar e padronizar a criação do relatório mensal de chamados do DeskManager, garantindo que os dados sejam filtrados e calculados de forma precisa e consistente, reduzindo o tempo gasto em tarefas manuais e eliminando erros humanos.

Público-Alvo
Analistas, assistentes e gerentes de suporte técnico ou atendimento que utilizam o DeskManager e precisam gerar relatórios detalhados com indicadores específicos para apresentar à gestão. O sistema é especialmente útil para quem busca otimizar o fluxo de trabalho e ter mais segurança na precisão dos dados.

Como Usar
Siga este guia passo a passo para gerar seu relatório completo.

Parte 1: Extração e Preparação da Planilha (Manual)
Extraia o relatório do DeskManager:

Acesse o sistema DeskManager e navegue até Configurações >> Relatório de Chamados.

Exporte o relatório no formato de planilha (.xlsx, .xls ou .csv).

Prepare o arquivo para o aplicativo:

Abra a planilha no Excel ou em outro editor.

Remova as linhas 1, 2 e 3 que contêm títulos e informações extras do relatório do DeskManager. A primeira linha do arquivo deve ser o cabeçalho das colunas.

Substitua o nome do grupo de categoria Desenvolvimento - Modulo Financeiro para Suporte - SASC CONNECT na coluna Grupo da Auto-Categoria Nome (coluna J).

Parte 2: Geração do Relatório (Automático)
Acesse o Aplicativo:

Abra o navegador e acesse o link: https://wallacegol.github.io/relatorio-deskmanager/

Carregue sua planilha:

Clique na área de upload ou arraste e solte o arquivo da planilha que você preparou.

Processe os dados:

Clique no botão "Processar Relatório" e aguarde a análise ser concluída.

Explore as novas funcionalidades com IA:

Para cada chamado nas tabelas, você pode usar os novos botões para:

Gerar Resumo ✨: Cria um resumo conciso da descrição do chamado para agilizar a leitura.

Sugerir Próximos Passos ✨: Analisa a descrição do chamado em backlog e sugere 3 passos lógicos para a resolução.

Exporte os resultados:

Após a visualização, clique em "Exportar para XLSX".

O aplicativo gerará um arquivo .xlsx com todas as tabelas em abas separadas, prontas para serem usadas.

Regras de Análise
O aplicativo aplica as seguintes regras de cálculo:

Total de Chamados por Grupo: Contagem simples de todos os chamados por cada Grupo da Auto-Categoria Nome (coluna J).

Atendidos pelo SAC: A contagem de chamados onde o Grupo da Auto-Categoria Nome (coluna J) é Suporte - SASC, Suporte - SASC CONNECT ou Suporte - SASC CM e a Fantasia (coluna L) não é COOPSASC.

Backlog Triagem: Contagem de chamados onde o Grupo da Auto-Categoria Nome (J) e o Nome do Status (I) correspondem aos critérios definidos, e o Nome do Operador (M) é Wallace, Mirlaine ou Agata.

Resolvidos Serviços: Contagem de chamados onde o Grupo da Auto-Categoria Nome (J), Nome do Tipo de Ocorrência (N), Nome do Status (I) e Fantasia (L) se encaixam nas regras, e o Nome do Operador (M) é Agata, Mirlaine ou Wallace.

Tecnologias
Frontend: HTML5, Tailwind CSS

Processamento de Planilhas: SheetJS/XLSX.js

Inteligência Artificial: Gemini API (para resumo e sugestões)
