# Casos de Teste – Módulo de Cursos

## Funcionalidade: Gerenciar cursos

### Cenário: Criar curso com sucesso
**Dado que** o usuário está na página de criação de curso  
**Quando** ele preencher o título, descrição e imagem  
**E** clicar em "Salvar"  
**Então** o sistema deve exibir a mensagem **"Curso criado com sucesso"**  
**E** o novo curso deve aparecer na listagem  

---

### Cenário: Criar curso com campos obrigatórios vazios
**Dado que** o usuário está na página de criação de curso  
**Quando** ele deixar algum campo obrigatório vazio  
**E** clicar em "Salvar"  
**Então** o sistema deve exibir **mensagens de erro**  

---

### Cenário: Listar cursos cadastrados
**Dado que** existem cursos cadastrados  
**Quando** o usuário acessar a página de cursos  
**Então** o sistema deve exibir **a lista de cursos com título e imagem**  

---

### Cenário: Excluir curso
**Dado que** o usuário está na listagem de cursos  
**Quando** ele clicar em **"Excluir"** em um curso  
**E** confirmar a exclusão  
**Então** o sistema deve **remover o curso da listagem**  
**E** exibir a mensagem **"Curso excluído com sucesso"**
