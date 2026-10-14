# Lar Ternura · Sistema de Doações

Plataforma web que mostra, em tempo real, o que a **Associação Lar Ternura** mais precisa e permite que doadores agendem a entrega dos itens. Projeto Integrador em Computação II da **UNIVESP**.

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-1e5aa8)
![Acessibilidade](https://img.shields.io/badge/acessibilidade-WCAG%202.1%20AA-067647)
![Licença](https://img.shields.io/badge/uso-acad%C3%AAmico-4a5871)

## O problema

A Associação Lar Ternura, organização do terceiro setor na Zona Oeste de São Paulo, depende de doações de alimentos, higiene e limpeza. Sem uma forma simples de comunicar o que falta, chegam itens que já sobram enquanto outros, urgentes, ficam em falta, e as entregas acontecem sem aviso.

## A solução

**Para quem doa:**

- Um **termômetro de necessidades**, com os itens mais urgentes primeiro e quanto falta para cada meta.
- **Agendamento da entrega** em horários com vagas, com um link privado para consultar, remarcar ou cancelar.

**Para a equipe da ONG:**

- Um **painel** para registrar as doações que chegaram, inclusive entregas parciais e espontâneas.
- **Gestão de metas e produtos**, com histórico preservado: nenhuma entrega é apagada, só estornada com motivo.

A interface foi pensada para um público mais velho e para uma equipe sem formação técnica: fonte de alta legibilidade, contraste reforçado, áreas de toque amplas e navegação completa por teclado.

## Repositórios

| Repositório | Conteúdo |
| --- | --- |
| [`sistema-doacoes`](https://github.com/univesp-pi-lar-ternura/sistema-doacoes) | Aplicação completa: API (`backend/`), interface (`frontend/`) e scripts do banco |

## Tecnologias

| Camada | Escolha |
| --- | --- |
| Interface | React, Tailwind CSS, Vite |
| API | Node.js, Express, contrato OpenAPI 3.0 |
| Banco de dados | PostgreSQL no Neon |
| Hospedagem da API | Render |
| Testes | Node test runner e PGlite (API), Vitest e axe-core (interface) |

## Equipe

| Integrante | Principais responsabilidades |
| --- | --- |
| Helena Ciorra ([@helenaciorra](https://github.com/helenaciorra)) | Liderança, infraestrutura e repositório, interface (termômetro e painel da ONG) |
| Anderson Loureiro ([@Anderson-MML](https://github.com/Anderson-MML)) | API REST, autenticação, prototipagem e wireframes |
| Vinicius Bica ([@vinbicca](https://github.com/vinbicca)) | Modelagem e scripts do banco de dados, integração com API externa, acessibilidade |
| Viviane Borba ([@viviane-borba](https://github.com/viviane-borba)) | Definição da stack, testes e documentação da API, responsividade |
| Ademir Stefanski ([@AdemirStefanski](https://github.com/AdemirStefanski)) | Relacionamento com a ONG e visitas de validação |

## Como trabalhamos

- **`main`** recebe apenas código integrado e testado; dela sai a publicação.
- **`develop`** concentra a integração das funcionalidades.
- Cada tarefa vive numa branch **`feature/*`** e entra na `develop` por Pull Request, com revisão de outro integrante.
- Ninguém faz commit direto na `main` nem na `develop`.

## Contexto acadêmico

Projeto Integrador em Computação II (PJI240), turma DRP14-A2026S2-T005, Universidade Virtual do Estado de São Paulo (UNIVESP), 2º semestre de 2026.

Os dados exibidos em ambientes de demonstração são **fictícios** e não representam necessidades reais da ONG.
