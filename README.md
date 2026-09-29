<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=210&section=header&text=João%20Davi&fontSize=52&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Full%20Stack%20Developer%20·%20Analista%20de%20Sistemas&descAlignY=56&descSize=18" alt="João Davi — Full Stack Developer" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/joaofranco02/joaofranco02/main/typing.svg" alt="Sistemas em produção na PMPA · Next.js + Fastify + PostgreSQL + Redis · Mestrando em Ciência da Computação (UFPA) · AWS Certified Cloud Practitioner" />
</p>

<p align="center">
  <a href="https://francodev.online"><img src="https://img.shields.io/badge/Portfólio-francodev.online-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfólio"></a>
  <a href="https://www.linkedin.com/in/jo%C3%A3o-franco-ab9179258/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:seuemail@dominio.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

## 👨‍💻 `whoami`

```ts
const joao = {
  cargo: "Full Stack Developer @ Polícia Militar do Pará",
  local: "Belém, PA 🇧🇷",
  emProducao: ["Boletim Acadêmico", "SGD", "Gerador de Contratos", "Plataforma EAD", "PICC"],
  formacao: "Mestrado em Ciência da Computação — UFPA (em andamento)",
  certificacoes: ["AWS Certified Cloud Practitioner"],
  aprendendoAgora: ["Java", "Angular"],
  filosofia: "Resolver problemas reais com código que o próximo dev consiga entender.",
} as const;
```

Construo sistemas internos que estão **em produção atendendo o efetivo da PMPA** — do frontend ao backend, passando por filas, infraestrutura e observabilidade. Não é projeto de tutorial: é software com usuário de verdade, deploy de verdade e bug de verdade às 8h da manhã. 😅

---

## 🏗️ Por dentro de um sistema em produção

O **[Sistema de Boletim Acadêmico](https://boletimacademico.pm.pa.gov.br)** em uma visão simplificada:

```mermaid
flowchart LR
    U["👮 Usuários"] --> FE["Next.js + React<br/>shadcn/ui · Zustand · RHF"]
    FE -->|REST| API["Fastify API<br/>Zod · Prisma"]
    API --> DB[("PostgreSQL")]
    API --> C[("Redis")]
    API -->|enfileira| Q["BullMQ<br/>jobs assíncronos"]
    Q --> C
    Q --> DB
```

> Validação de ponta a ponta com **Zod** (formulário → API), processamento pesado fora do ciclo de request com **BullMQ**, e **Prisma** tipando o acesso ao banco.

---

## 🚀 Projetos

### 🏛️ Em produção — PMPA
<sub>Código institucional (privado). Links levam aos sistemas no ar.</sub>

| | Projeto | O que resolve | Stack |
|---|---|---|---|
| 📘 | **[Boletim Acadêmico](https://boletimacademico.pm.pa.gov.br)** | Gestão de notas e boletins acadêmicos militares | Next.js · TypeScript · Fastify · Prisma · PostgreSQL · Redis · BullMQ |
| 👩‍🏫 | **[SGD](https://sgd.pm.pa.gov.br)** | Cadastro e gestão dos docentes da corporação | React · Vite · TypeScript · shadcn/ui |
| 📄 | **Gerador de Contratos** | Automatiza a geração de contratos administrativos | Django · FastAPI · PostgreSQL · Redis · Celery · Docker |
| 🎓 | **[Plataforma EAD](https://ead.pm.pa.gov.br)** | Ambiente virtual de capacitação do efetivo | Moodle · PHP · MariaDB · Apache · Nginx · Linux |
| 🪖 | **PICC** | Classificação por níveis de formação militar | PostgreSQL |

<details>
<summary><b>💼 Projetos pessoais & freelance</b></summary>
<br>

| Projeto | O que é | Stack | Link |
|---|---|---|---|
| 🎮 Jogo 2D/3D | Projeto pessoal de game dev | C# · Unity | [Repo](https://github.com/joaofranco02/projeto-unity) |
| 🌐 Studio Soares Deize | Site institucional para cliente | HTML · CSS · JavaScript | [Repo](https://github.com/joaofranco02/projeto-spa) |

</details>

---

## 🧰 Stack

<table>
  <tr>
    <td align="center" width="130"><b>Frontend</b></td>
    <td><img src="https://skillicons.dev/icons?i=ts,react,nextjs,tailwind,html,css,js" /></td>
  </tr>
  <tr>
    <td align="center"><b>Backend</b></td>
    <td><img src="https://skillicons.dev/icons?i=nodejs,nestjs,py,django,fastapi" /> <img src="https://img.shields.io/badge/Fastify-000000?style=for-the-badge&logo=fastify&logoColor=white" height="40" /></td>
  </tr>
  <tr>
    <td align="center"><b>Dados & Filas</b></td>
    <td><img src="https://skillicons.dev/icons?i=postgres,redis,mongodb,prisma" /> <img src="https://img.shields.io/badge/BullMQ-DC382D?style=for-the-badge" height="40" /> <img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white" height="40" /></td>
  </tr>
  <tr>
    <td align="center"><b>DevOps & Obs.</b></td>
    <td><img src="https://skillicons.dev/icons?i=docker,githubactions,nginx,linux,aws,grafana,prometheus" /> <img src="https://img.shields.io/badge/Loki-F5A623?style=for-the-badge&logo=grafana&logoColor=white" height="40" /></td>
  </tr>
</table>

<details>
<summary><b>➕ Outras ferramentas</b></summary>
<br>

![Zod](https://img.shields.io/badge/Zod-3E67B1?style=flat-square&logo=zod&logoColor=white)
![React Hook Form](https://img.shields.io/badge/React_Hook_Form-EC5990?style=flat-square&logo=reacthookform&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-433E38?style=flat-square)
![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000?style=flat-square&logo=shadcnui&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white)
![Apache](https://img.shields.io/badge/Apache-D22128?style=flat-square&logo=apache&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Unity](https://img.shields.io/badge/Unity-000000?style=flat-square&logo=unity&logoColor=white)

</details>

---

## 🔭 Agora mesmo

- ☕ Aprofundando **Java**
- 🅰️ Fechando a lacuna em **Angular**
- 🎓 Pesquisando no **Mestrado em Ciência da Computação (UFPA)**
- 💬 Aberto a conversar sobre **backend, sistemas em produção e arquitetura**

---

## 📊 Atividade

> A maior parte do meu código de produção vive em repositórios privados — isto aqui é só a ponta do iceberg. 🧊

<p align="center">
  <img src="https://raw.githubusercontent.com/joaofranco02/joaofranco02/main/metrics.svg" alt="Stats e atividade do João">
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/joaofranco02/joaofranco02/output/github-snake-dark.svg" />
    <img alt="Cobrinha comendo as contribuições" src="https://raw.githubusercontent.com/joaofranco02/joaofranco02/output/github-snake.svg" />
  </picture>
</p>

---

<p align="center">
  ⭐ Curtiu algum projeto? Deixa uma estrela ou me chama no <a href="https://www.linkedin.com/in/jo%C3%A3o-franco-ab9179258/">LinkedIn</a>.
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=110&section=footer" />
</p>
