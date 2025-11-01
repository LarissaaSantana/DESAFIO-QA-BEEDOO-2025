### Decisões tomadas para a criação da Historia de usuário.

Foi usada a metodologia de **teste exploratório** para entender melhor o funcionamento do sistema e levantar informações reais. Durante o processo, explorei diferentes partes da aplicação, usei ferramentas do navegador (como console e network) e observei o comportamento das funções. Isso ajudou a identificar pontos importantes e reunir dados úteis para montar a user story com mais clareza e base técnica.

As decisões foram tomadas com base nos resultados do teste e na minha experiência como QA durante o estágio. Essa vivência ajudou a enxergar possíveis falhas e pensar em diferentes cenários, incluindo erros e exceções. Assim, a user story foi construída de forma objetiva e prática, garantindo que refletisse o que o usuário realmente precisa e trazendo valor ao produto final.

### HU Criar curso
**Dado que** o usuário está na página da listagem de curso
**Quando** clicar no botão "CADASTRAR CURSO"
**E** preencher todos campos corretamente  
**E** clicar em "CADASTRAR CURSO"  
**Então** o sistema deve exibir a mensagem **"Curso cadastrado com sucesso"**  
**E** o novo curso deve aparecer na listagem  

### Detalhamento dos campos 
| *Campo* | *Descrição do campo* | *Máscara* | *Obrigatório* | *Editável* | *Tipo* | *Tam* |
|-----------|------------------------|:-----------:|:---------------:|:------------:|:--------:|:-------:|
| Nome do curso |Campo para adicionar nome ao curso | N/A | S | S | Textual | N/A |
| Descrição do curso |Campo para adicionar descrição do curso | N/A | S | S | Textual | N/A |
| Instrutor |Campo para adicionar nome do Instrutor | N/A | S | S | Textual | N/A |
| Url da imagem de capa |Campo para adicionar url da imagem capa | N/A | S | S | Link | N/A |
| Data de Inicio |Campo para adicionar Data de Inicio | N/A | S | S | Date | N/A |
| Data de Fim |Campo para adicionar Data de Fim | N/A | S | S | Date | N/A |
| Numero de vagas |Campo para adicionar numero de vagas | N/A | S | S | Numerico | N/A |
| Tipo de Curso |Caixa de seleção para selecionar o tipo de curso presencial/online | N/A | S | S | Caixa de seleção | N/A |
|Endereço/Link de descrição |Campo de endereço/Link de descrição | N/A | S | S | textual/Link | N/A |

### Criterios de aceitação

Ao clicar no botão **salvar curso** o sistema deve fazer a validação de todos os campos.

No seletor **Tipo de curso** selecione uma das opções:



**Presencial** ao selecionar essa opção é necessario informar o endereço.  
**Online** ao selecionar essa opção é necessario informar o link. 


---

### HU Listar cursos cadastrados
**Dado que** existem cursos cadastrados  
**Quando** o usuário acessar a página de cursos  
**Então** o sistema deve exibir a listagem de **Cursos em cads**  

### Criterios de aceitação

Cada card de curso deve seguir uma ordem ASC onde deve conter a imagem de capa, modalidade, nome do curso, descrição, data de inicio e de fim, numero de vagas e botão de **EXCLUIR CURSO** onde sua funcionalidade esta descrita na HU **Excluir curso**.


---

### HU Excluir curso
**Dado que** o usuário está na listagem de cursos  
**Quando** clicar no botão **"EXCLUIR CURSO"** em um card
**Então** o sistema deve **remover o curso da listagem**  
**E** exibir a mensagem **"Curso excluído com sucesso"**

### Criterios de aceitação

Ao clicar no botão **EXCLUIR CURSO** o sistema devera excluir o curso do banco de dados e apresentar mensagem de **Curso excluido com sucesso**
