[output_PageInterim.txt](https://github.com/user-attachments/files/17317281/output_PageInterim.txt)# DesafioPageInterim

Este repositório faz parte da etapa de desafio técnico do processo seletiovo da empresa Page Interim.

# Considerações sobre o projeto:

Todos o fluxos foi desenvolvido respeitando os requisitos descritos no arquivo .pdf enviado, ou seja, mesmo que existam diferentes formas de aplicar os conceitos descritos no desafio para otimizar o processamento e uso de licença como o framework de Dispatcher e Performer, entre outros, optei por respeitar o que os requisitos estavam avaliando como a utilização do Reframework.

A automação está funcional e pronta para uso, abaixo desta mensagem inseri os emails de resultado de processamento para casos de sucesso e falha. O desenvolvimento foi realizado utilizando boas práticas da UiPath. Caso esse fosse um caso real de uma automação no pipeline eu adicionaria uma pequena melhoria no Retry em caso de System Exception durante o download dos arquivos para a automação se recuperar a partir do último arquivo já baixado, desta forma o custo de licença alocada seria reduzido ampliando o retorno de investimento (ROI) da mesma. 

Optei pelo Reframework por questões avaliativas do processo e de monitoramento do processo em produção pelos mecaniscos que o API Server da UiPath oferece para criação de dashboards, utilizando o Swagger do orquestrador da organização como ferramenta de apoio é possível observar a quantidade de endpoints disponíveis para esse monitoramento com o uso de ferramentas como Grafana ou DataDog. Toda a configuração de assets pode ser observada no arquivo Config.xlsx seguindo o Reframework. 

# Resultados:

- Email de sucesso (HTML, CSS)

![image](https://github.com/user-attachments/assets/74f28080-10d4-4d05-a9e6-6b75f4612111)


- Email de falha (HTML, CSS)

![image](https://github.com/user-attachments/assets/49bea446-da5a-4caa-943f-f9d2c143517a)


- Assets no Orquestrador (seguindo boas práticas de nomenclatura)

![image](https://github.com/user-attachments/assets/94f6c3b7-55bc-432a-ba91-42967800a639)


- Fila no Orquestrador (existem mais evidências mas deletei itens desnecessários)

![image](https://github.com/user-attachments/assets/b2f166e1-bc15-4a13-812a-d784ddb9bfe4)


- Logs de processamento
[Uploading output10/09/2024 14:16:39 => [Debug] Debug started for file: Main
10/09/2024 14:16:45 => [Info] DesafioUiPathPageInterim execution started
10/09/2024 14:16:45 => [Info] The primary screen resolution is: 1366 x 768
10/09/2024 14:16:45 => [Debug] Initializing settings...
10/09/2024 14:16:51 => [Debug] Killing processes...
10/09/2024 14:16:51 => [Debug] Opening applications...
10/09/2024 14:16:51 => [Debug] Audit: Using Web App. Browser: Chrome URL: https://dados.gov.br/dados/conjuntos-dados/cadastro-nacional-da-pessoa-juridica---cnpj
10/09/2024 14:16:52 => [Info] Portal de Dados successfully opened.
10/09/2024 14:16:54 => [Info] Última alteração: 18/09/2024 16:35:29
10/09/2024 14:16:54 => [Info] String format: 18/09/2024 16:35:29
10/09/2024 14:16:54 => [Info] Last Update Datetime format: 09/18/2024 16:35:29
10/09/2024 14:16:54 => [Info] Last Extraction Datetime format: 09/17/2024 16:35:29
10/09/2024 14:16:54 => [Info] Inserting Queue Item...
10/09/2024 14:16:55 => [Info] Successfully added queue item
10/09/2024 14:16:55 => [Info] Get the transaction item
10/09/2024 14:16:55 => [Info] Transaction Started
10/09/2024 14:16:55 => [Info] Processing Transaction Number: 1
10/09/2024 14:16:55 => [Info] Started Process
10/09/2024 14:16:55 => [Debug] Audit: Using Web App. Browser: Chrome URL: https://dados.gov.br/dados/conjuntos-dados/cadastro-nacional-da-pessoa-juridica---cnpj
10/09/2024 14:16:57 => [Debug] Audit: Using Web App. Browser: Chrome URL: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/?C=N;O=D
10/09/2024 14:16:58 => [Debug] Audit: Extract Data. From: <html app='chrome.exe' url='https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/?C=N;O=D' />
10/09/2024 14:16:59 => [Info] Waiting download to complete
10/09/2024 14:17:04 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Cnaes.zip
10/09/2024 14:17:04 => [Info] Waiting download to complete
10/09/2024 14:19:36 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Empresas1.zip
10/09/2024 14:19:37 => [Info] Waiting download to complete
10/09/2024 14:21:28 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Empresas2.zip
10/09/2024 14:21:29 => [Info] Waiting download to complete
10/09/2024 14:23:09 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Empresas3.zip
10/09/2024 14:23:10 => [Info] Waiting download to complete
10/09/2024 14:24:34 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Empresas4.zip
10/09/2024 14:24:35 => [Info] Waiting download to complete
10/09/2024 14:26:10 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Empresas5.zip
10/09/2024 14:26:11 => [Info] Waiting download to complete
10/09/2024 14:28:43 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Empresas6.zip
10/09/2024 14:28:44 => [Info] Waiting download to complete
10/09/2024 14:31:16 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Empresas7.zip
10/09/2024 14:31:17 => [Info] Waiting download to complete
10/09/2024 14:34:26 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Empresas8.zip
10/09/2024 14:34:27 => [Info] Waiting download to complete
10/09/2024 14:44:17 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Empresas9.zip
10/09/2024 14:44:17 => [Info] Waiting download to complete
10/09/2024 14:44:21 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Motivos.zip
10/09/2024 14:44:22 => [Info] Waiting download to complete
10/09/2024 14:44:26 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Municipios.zip
10/09/2024 14:44:27 => [Info] Waiting download to complete
10/09/2024 14:44:31 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Naturezas.zip
10/09/2024 14:44:31 => [Info] Waiting download to complete
10/09/2024 14:44:35 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Paises.zip
10/09/2024 14:44:36 => [Info] Waiting download to complete
10/09/2024 14:44:40 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Qualificacoes.zip
10/09/2024 14:44:41 => [Info] Waiting download to complete
10/09/2024 14:48:06 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Socios1.zip
10/09/2024 14:48:06 => [Info] Waiting download to complete
10/09/2024 14:50:43 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Socios2.zip
10/09/2024 14:50:44 => [Info] Waiting download to complete
10/09/2024 14:53:17 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Socios3.zip
10/09/2024 14:53:18 => [Info] Waiting download to complete
10/09/2024 14:55:03 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Socios4.zip
10/09/2024 14:55:03 => [Info] Waiting download to complete
10/09/2024 14:57:11 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Socios5.zip
10/09/2024 14:57:11 => [Info] Waiting download to complete
10/09/2024 14:59:32 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Socios6.zip
10/09/2024 14:59:32 => [Info] Waiting download to complete
10/09/2024 15:02:20 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Socios7.zip
10/09/2024 15:02:21 => [Info] Waiting download to complete
10/09/2024 15:04:37 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Socios8.zip
10/09/2024 15:04:38 => [Info] Waiting download to complete
10/09/2024 15:07:03 => [Info] File downloaded and moved to the CNPJ Files folder: https://dadosabertos.rfb.gov.br/CNPJ/dados_abertos_cnpj/2024-09/Socios9.zip
10/09/2024 15:07:07 => [Info] Transaction Ended
10/09/2024 15:07:07 => [Info] Transaction Successful.
10/09/2024 15:07:07 => [Info] Get the transaction item
10/09/2024 15:07:07 => [Info] No Transaction Data
10/09/2024 15:07:07 => [Info] Process finished due to no more transaction data
10/09/2024 15:07:07 => [Info] Closing applications...
10/09/2024 15:07:16 => [Info] DesafioUiPathPageInterim execution ended in: 00:50:31
_PageInterim.txt…]()



