# Demanda Futebas – Versão 1 

## Informações sobre a demanda

O objetivo será desenvolver um sistema de cadastro de perfil de atletas amadores em busca de quadras/times de futebol. Após levantamento de requisitos junto ao cliente, listaremos as especificações a serem desenvolvidas pela equipe deback-end.

Importante salientar que o sistema será uma API Rest (Mais explicações) com autenticação por Json Web (Mais explicações)
Token (JWT).
O sistema deverá possuir uma documentação dos recursos disponíveis pela API (Mais explicações), para
servir de apoio a equipe de front-end (Mais explicações).


### Nesta primeira versão temos os seguintes requisitos a serem desenvolvidos:

# 1. Requisitos e Configurações
    • A API deverá ser configurada com o Timezone do país
    • A API deverá ser configurada com o Locale do país
    • A API deverá usar um sistema de auditoria
    • Registrar a data de criação e última modificação dos registros
    • Registrar o usuário que criou e o último que modificou um registro
    • Configurar o acesso a uma base de dados para o ambiente de desenvolvimento MySQL (inicialmente)
      
# 2. Requisitos / Jogadores(ras)
    • O(A) jogador(a) deverá ter um e-mail, o qual será usado como username (deve ser único)
    • O(A) jogador(a) deverá ter uma senha de 6 caracteres
    • O(A) jogador(a) deverá ter um perfil de jogador(a) .
    • O(A) jogador(a) poderá ser localizado pelo identificador gerado (nick único).
    • O(A) jogador(a) cadastrar seus atributos (habilidades, pontos fortes, perna que chuta, etc...).
    • O(A) jogador(a) , quando autenticado, poderá somente recuperar seus próprios atributos de usuário.
    • O(A) jogador(a) pode visualizar seus stauts na quadra/horário que joga.
    • O usuário poderá alterar a senha
      (Apenas quando estiver autenticado e somente o próprio usuário terá essa autorização)
    • Documentar todos os recursos criados.
    • Realizar testes de integração do tipo ponto a ponto (end-to-end) dos recursos criados.




# 3. Requisitos / Autenticação
    • Implementar um sistema de segurança e autenticação com JSON Web Token
    • Documentar o recurso de autenticação.
    • Realizar testes sobre o sistema de autenticação


# 4. Requisitos / Gestão de Quadra
 
    • O(A) administrador(a) pode cadastrar um horario  e um local que joga
    • O(A) administrador(a) cadastrar jogadores no horário da quadra 
    • O(A) administrador(a) pode marcar quais pagamentos foram feitos pelos jogadores(ras) da quadra. 
    • O(A) administrador(a) deve receber o telefone para contatar cada jogador(a) quando solicitar.
    • O(A) administrador(a) deve ter um controle de pagamentos mensais feitos para manter o horário da quadra.
    • O(A) administrador(a) deve pode elencar outros administradores para a quadra
    • OS(AS) administradores(ras) devem poder cadastrar as stauts dos jogadores. 

# 5. Requisitos / Gestão de Time
    • O(A) Presidente(a) pode agendar as informações sobre o horário que joga o seu grupo (inserir jogadores, horario e local da quadra)
    • O(A) Presidente(a) cadastrar jogadores no horário da quadra 
    • O(A) Presidente(a) oferecer pagamento para jogos pontuais  
    • O(A) Presidente(a) pode avaliar os jogadores que foram contratados



# 6. Requisitos / Geolocalização
    • A API deverá ter um modulo de geolocalização. 
    • A API deve possuir um endpoint (mais Explicações) para recuperar  latitude/longitude de determinado ponto do mapa.
    • O(A) jogador(a) pode buscar uma quadra próximo a sua localidade.
    • O(A) jogador(a) pode cadastrar o raio de busca de alerta de jogos. 
    • O(A) administrador(a) pode localizar as quadras em rua região
    • O(A) administrador(a) pode publica o horário de jogos do seu grupo (aluguel de goleiro)
    • O(A) administrador(a)pode publicar o interesse de montar um time na região selecionada.
    • O(A) presidente(a) pode localizar os jogos em rua região


# 7. Requisitos / Jogador Postar Lances, Gols e Texto

    • O(A) Jogador(a) pode postar texto(240 char), fotos e vídeos curtos.
    • O(A) Jogador(a) pode ter acesso ao feed.
    • O(A) jogador(a) pode criar um grupo de discussão em comum.
      


