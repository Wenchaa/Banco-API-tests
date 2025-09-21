[README.md](https://github.com/user-attachments/files/22454639/README.md)
# Banco API Tests

## 📌 Objetivo
Este projeto tem como objetivo **automatizar testes da API REST** do repositório [Banco API](https://github.com/juliodelimas/banco-api), garantindo que suas operações estejam funcionando corretamente.  
O foco principal é **contribuir com a qualidade das operações**, facilitando a validação de endpoints e a detecção de falhas de forma rápida e consistente.

---

## 🛠️ Stack utilizada
O projeto utiliza as seguintes tecnologias e bibliotecas:

- **[Node.js](https://nodejs.org/)** → Ambiente de execução
- **[Mocha](https://mochajs.org/)** → Framework de testes
- **[Chai](https://www.chaijs.com/)** → Biblioteca de assertions
- **[Supertest](https://github.com/visionmedia/supertest)** → Requisições HTTP para testar APIs
- **[Dotenv](https://github.com/motdotla/dotenv)** → Gerenciamento de variáveis de ambiente
- **[Mochawesome](https://github.com/adamgruber/mochawesome)** → Geração de relatórios em HTML

---

## 📂 Estrutura de diretórios

```
Banco-API-tests/
│── test/                 # Diretório com os testes automatizados
│   ├── transferencia.test.js/   # Testes específicos de transferências
│   ├── login.test.js/           # Testes específicos de login
│   └── ...
│── mochawesome-report/   # Relatórios em HTML (gerados após execução)
│── package.json          # Dependências e scripts
│── .env                  # Configurações de ambiente (não incluso no repositório)
```

---

## ⚙️ Arquivo `.env`
O arquivo `.env` **não está incluso no repositório** e precisa ser criado pelo usuário.  
Ele deve conter a URL base da API que será testada:

```env
BASE_URL=http://localhost:3000
```

> 🔑 Caso a API necessite autenticação, recomenda-se adicionar também o `TOKEN` ou configurar login automático nos testes.

---

## ▶️ Executando os testes

### 1. Instalar dependências
```bash
npm install
```

### 2. Executar todos os testes
```bash
npm test
```

### 3. Gerar relatório em HTML com Mochawesome
Após rodar os testes, um relatório será gerado em:

```
./mochawesome-report/mochawesome.html
```

Para abrir:
- No navegador → clique duas vezes no arquivo
- Ou rode:
```bash
npx mochawesome-merge ./mochawesome-report/*.json | npx mochawesome-report-generator
```

---

## 📚 Documentação das dependências
- [Mocha](https://mochajs.org/#getting-started)
- [Chai](https://www.chaijs.com/guide/styles/)
- [Supertest](https://github.com/visionmedia/supertest)
- [Dotenv](https://github.com/motdotla/dotenv#readme)
- [Mochawesome](https://github.com/adamgruber/mochawesome)

---

## 🤝 Contribuição
Este projeto é de caráter **educacional** e tem como finalidade contribuir para a **qualidade e confiabilidade das operações da API Banco**.  
Sugestões de melhorias são bem-vindas!  
