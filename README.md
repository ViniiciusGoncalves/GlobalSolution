# GlobalSolution

# Aviso ----- BUG
Após criar um pedido de doação atualizar o index.js do Home  para aparecer no código, não consegui dar um refresh após efetuar o cadastro....

# Link do video mostrando o front e o bug
url: https://www.youtube.com/watch?v=XbDZEwYbp_E&ab_channel=ViniciusGon%C3%A7alves

# Endpoints da API

UserController

<ul>
  <li>POST /api/users/donor - Cria um novo doador.</li>
  <ul>
    <li>Body: Doador object</li>
    <li>Response: ResponseEntity<Doador></li>
  </ul>
  <li>POST /api/users/help - Cria uma nova solicitação de ajuda.</li>
  <ul>
    <li>Body: PrecisandoAjuda object</li>
    <li>Response: ResponseEntity<PrecisandoAjuda></li>
  </ul>
  <li>POST /api/users/login - Faz login de usuário.</li>
  <ul>
    <li>Body: User object</li>
    <li>Response: ResponseEntity<User></li>
  </ul>
</ul>


DoacaoController

<ul>
  <li>GET /api/doacoes - Retorna todas as doações.</li>
  <ul>
    <li>Response: List<Doacao></li>
  </ul>
  <li>POST /api/doacoes - Cria uma nova doação.</li>
  <ul>
    <li>Body: DoacaoRequest object</li>
    <li>Response: Doacao</li>
  </ul>
  <li>PUT /api/doacoes/{id} - Atualiza uma doação existente com o ID fornecido.</li>
  <ul>
    <Li>Path Variable: id (Long)</li>
    <li>Body: DoacaoRequest object</li>
    <li>Response: ResponseEntity<Doacao></li>
  </ul>
</ul>

