# Classic-Phrases

ScreenMatch é uma aplicação web que exibe **frases famosas de séries e filmes**, permitindo que o usuário visualize aleatoriamente diferentes citações com personagens e imagens associadas. O projeto possui backend em **Java Spring Boot** e frontend em **HTML/CSS/JavaScript**, consumindo a API local para exibir os dados dinamicamente.

---

## 🛠 Tecnologias Utilizadas

### Backend
- Java 21
- Spring Boot
- Spring Data JPA
- PostgreSQL
- Maven

### Frontend
- HTML5
- CSS3
- JavaScript (ES6 Modules)
- Fetch API

---

## 📂 Estrutura do Projeto

### Backend (`screenmatch`)
- `ScreenmatchApplication.java` – Classe principal do Spring Boot.
- `Frase.java` – Entidade JPA representando uma frase de série/filme.
- `FraseDTO.java` – Record para transporte de dados da entidade.
- `FraseRepository.java` – Repositório com método customizado para buscar frase aleatória.
- `FraseService.java` – Serviço que retorna `FraseDTO` ao controlador.
- `FraseController.java` – Controlador REST expondo endpoint `/series/frases`.
- `CorsConfiguration.java` – Configuração CORS permitindo requisições do frontend.

### Frontend (`/frontend`)
- `index.html` – Estrutura da página com cabeçalho, área de frases e botão de sortear.
- `style.css` – Estilos visuais (não enviado, mas referenciado).
- `scripts/getDados.js` – Função para consumir API do backend.
- `scripts/index.js` – Manipula DOM e exibe frases aleatórias, integrando com `getDados`.

---

## 🚀 Funcionalidades

- Exibe **frases aleatórias** de séries e filmes.
- Mostra o **personagem** que citou a frase.
- Exibe a **imagem (poster)** associada à série ou filme.
- Permite ao usuário **sortear novas frases** clicando no botão "Ver outras frases...".
- Comunicação frontend-backend via **Fetch API**.

---

## ⚙ Como Executar

### Backend

1. Clone o repositório:
```bash
git clone https://github.com/Kaio-0708/classic-phrases.git

2.cd classic-phrases

3.Configure o PostgreSQL com uma base de dados chamada screenmatch (ou ajuste o application.properties).

4.Rode a aplicação Spring Boot:
mvn spring-boot:run

5.O backend estará disponível em http://localhost:8081. 
```

## 📸 Demonstração

Link:  https://drive.google.com/file/d/1v0Fp-yM62UXo1Dj1DvYTvF7DHWAvYCmo/view?usp=drive_link

Ao abrir a aplicação, você verá:

- Imagem da série/filme
- Título
- Frase aleatória
- Nome do personagem
- Botão para sortear novas frases

## 👨‍💻 Autor

Kaio Vitor - [GitHub](https://github.com/Kaio-0708)



