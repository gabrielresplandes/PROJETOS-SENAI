# PROJETOS-SENAI
### *Hotel Acapulco - Website Oficial*
##### Para melhor acesso ao Website observe as instruções ao final dessa documentação

---

#### 1. Estrutura Geral
O sistema é composto por múltiplas páginas HTML, estilizadas por arquivos CSS e com funcionalidades implementadas em JavaScript. Seu objetivo é representar o site de um hotel, com foco na experiência do usuário, funcionalidades administrativas e integração com formulários de terceiros.

---

#### 2. Componentes do Sistema

##### 2.1. Página Principal (index.html)

**Descrição:** 
Apresenta as informações iniciais sobre o hotel, incluindo um catálogo de quartos, promoções e a seção de reservas.

- **Seções Principais:**
  - **Header:** Inclui o logotipo, nome do hotel e uma barra de navegação com links para outras páginas.
  - **Catálogo de Quartos:** Mostra quatro tipos de acomodações disponíveis, cada uma com imagem, descrição, preço e botão "VER MAIS".
  - **Promoção VIP:** Convida os usuários a se cadastrarem no programa de fidelidade.
  - **Reservas:** Exibe as informações de contato do hotel e um botão para acessar o formulário de reservas.
  - **Footer:** Contém informações de direitos autorais.

**Observações Técnicas:**
- **Acessibilidade:** Uso do atributo `alt` em imagens para melhorar a acessibilidade.
- **Responsividade:** Implementada para adaptar-se a diferentes tamanhos de tela com CSS Flexbox.
- **JavaScript:** Função `scrollToSection(id)` usada para navegação suave entre seções.

---

##### 2.2. Página "Sobre Nós" (sobreNos.html)

**Descrição:**  
Apresenta informações detalhadas sobre o hotel, incluindo histórico e descrição das acomodações.

- **Seções Principais:**
  - **Introdução:** Breve história do hotel.
  - **Detalhamento das Acomodações:** Destaca os diferenciais das acomodações.

**JavaScript:**
- Função `scrollToNext()` para rolar suavemente para a próxima seção.

---

##### 2.3. Página de Login (login.html)

**Descrição:**
Permite que os administradores acessem a intranet para gerenciar reservas.

- **Funcionalidades:**
  - Validação de usuário e senha.
  - Redirecionamento para a página de intranet em caso de sucesso.
  - Feedback para erros no login.

**JavaScript:**
- Validação do login com comparação de valores fixos (`validUser` e `validPassword`).

**Estilização:**
- Formulário centralizado com campos estilizados.
- Foco nos campos para melhor experiência visual.

---

##### 2.4. Página da Intranet (intranet.html)

**Descrição:**  
Permite o cadastro, visualização e exclusão de reservas e inclui um botão de logout para redirecionamento à página inicial.

- **Funcionalidades:**
   Cadastro de reservas com validação de campos:
      - Nome do cliente deve conter apenas letras e espaços.
      - Dias e valor da diária devem ser maiores que zero.
      - Atualização de reservas: Cálculo de valores acumulados
      - Opção de "Dar Baixa" em reservas, removendo-as da lista.
   
   Logout:
      - Botão de logout posicionado no **header**.
      - Ao ser clicado, redireciona o usuário para a página inicial do site (index.html)

      **JavaScript(logout)**
      - Função associada ao botão **#logout-btn** que exibe um alerta ao usuário e redireciona para a página inicial

**JavaScript:**
- Manipulação dinâmica do DOM para exibir reservas.
- Validação com regex para entrada de nomes.

**Estilização:**
- Formulário com design simples e acessível.
- Lista de reservas estilizada com botões para exclusão.

---

#### 3. Estilização

##### **Arquivos CSS:**
- **index.css:** Focado na estilização da página principal. Inclui:
  - Background com imagem fixa.
  - Estilo das seções e elementos como botões e cards.
- **sobreNos.css:** Configurações específicas para a página "Sobre Nós", com design clean e responsivo.
- **login.css:** Estilo moderno para o formulário de login, com cores e layout atraentes.
- **intranet.css:** Layout funcional para cadastro e exibição de reservas.

**Técnicas de Estilização:**
- Uso extensivo de `flexbox` para layout responsivo.
- Paleta de cores consistente (tons de verde, preto e branco).
- Transições suaves para botões e elementos interativos.

---

#### 4. Funcionalidades em JavaScript

##### **4.1. Funções Utilizadas:**
- **`scrollToSection(id)` e `scrollToNext()`**: Rolagem suave para melhorar a navegação.
- **Validação de Formulários:**
  - Uso de regex para garantir dados consistentes.
- **Manipulação do DOM:** 
  - Adição, atualização e exclusão de elementos como listas de reservas.
- **Redirecionamento em Login:**
  - `window.location.href` para navegação entre páginas.

---

#### 5. Boas Práticas Implementadas

- **SEO:**
  - Uso de meta tags como `viewport` e `charset`.
  - Títulos específicos para cada página.
- **Acessibilidade:**
  - Textos alternativos (`alt`) em imagens.
  - Cores contrastantes para melhor leitura.
- **Código Limpo:**
  - Identação correta e nomes de classes intuitivos.
  - Separação de responsabilidades entre HTML, CSS e JavaScript.

---

#### 6. Pontos de Melhorias

- **Segurança:**
  - Implementar autenticação segura no login (exemplo: hashing de senhas).
- **Manutenção de Estado:**
  - Adicionar persistência para reservas usando localStorage ou integração com backend.
- **Acessibilidade Adicional:**
  - Uso de `aria-labels` e descrição para navegação em leitores de tela.
- **Modularização:**
  - Dividir o código JavaScript em módulos para maior clareza e reutilização.

---

### Instruções

 - Ao realizar o acesso dos arquivos, acesse o live server pelo index.html

 - Para acessar a intranet utilize o **login: admin** e a **senha: 12345**.

## Créditos
   - [@gabrielresplandes](https://github.com/gabrielresplandes) - Criador do projeto
   - [@vitinhozy](https://github.com/vitinhozy) - Melhorias de interface e demais ajustes 