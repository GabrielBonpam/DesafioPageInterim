# DesafioPageInterim

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
[output_PageInterim.txt](https://github.com/user-attachments/files/17317281/output_PageInterim.txt)


