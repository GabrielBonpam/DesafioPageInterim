# DesafioPageInterim

Este repositório faz parte da etapa de desafio técnico do processo seletivo da empresa Page Interim.

# Considerações sobre o projeto:

Todos o fluxos foram desenvolvidos respeitando os requisitos descritos no arquivo .pdf enviado como base do projeto, ou seja, mesmo que existam diferentes formas de aplicar os conceitos descritos no desafio para otimizar o processamento e uso de licença como o framework de Dispatcher e Performer, entre outros, optei por respeitar o que os requisitos estavam avaliando como a utilização do Reframework.

A automação está funcional e pronta para uso, abaixo desta mensagem inseri os emails de resultado de processamento para casos de sucesso e falha, entre outros itens. O desenvolvimento foi realizado utilizando boas práticas da UiPath. Caso esse fosse um caso real de uma automação no pipeline eu adicionaria uma pequena melhoria no Retry em caso de System Exception durante o download dos arquivos para a automação se recuperar a partir do último arquivo já baixado, desta forma o custo de licença alocada seria reduzido ampliando o retorno de investimento (ROI) da mesma. 

Optei pelo Reframework com os mecanismos de Retry ativados por questões avaliativas do processo e de monitoramento do processo em produção pelos mecanismos que o API Server da UiPath oferece para criação de dashboards, utilizando o Swagger do orquestrador da organização como ferramenta de apoio é possível observar a quantidade de endpoints disponíveis para esse monitoramento com o uso de ferramentas como Grafana ou DataDog. Toda a configuração de assets pode ser observada no arquivo Config.xlsx seguindo o Reframework ou no print abaixo, os logs da automação também se encontram no final deste arquivo. Como existem arquivos muito grandes com cerca de 1.3GB na base de dados eu removi os arquivos maiores durante os testes devido ao prazo de entrega, mas tive a oportunidade de executar com todos os arquivos e a automação está toda funcional, porém nos logs da última execução vocês podem notar a falta dos arquivos maiores no processamento.

Observações técnicas: Não encontrei desafios técnicos evidentes durante o desenvolvimento, os seletores foram aplicados de forma dinâmica para que se adaptem as tabelas no site do Governo como boa prática. O único problema encontrado durante o desenvolvimento foi o download dos arquivos maiores devido ao prazo de entrega.

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


