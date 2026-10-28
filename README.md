# Corrige Aí

> **Mais cidade. Menos problema.**

Aplicativo Android para cidadãos denunciarem, registrarem e mapearem problemas urbanos (buracos, iluminação pública, lixo, calçadas danificadas etc.), facilitando a comunicação com os responsáveis pela manutenção da cidade.

Projeto Integrado Mobile, UNICEPLAC (Centro Universitário do Planalto Central), Gama-DF, 2026.

## Funcionalidades previstas

- Cadastro e login (e-mail/senha, Google e Apple)
- Registro rápido de denúncias com foto e localização (geolocalização)
- Classificação das denúncias por categoria
- Mapa com as ocorrências registradas
- Acompanhamento de status: registrada, em análise, em andamento e resolvida
- Identificação das regiões com mais problemas
- Incentivo à participação popular

## Equipe

| Integrante | Papel |
|---|---|
| Thyago da Fonseca Almeida | A definir |
| Marcelo de Jesus Pereira da Silva Neto | A definir |
| Carlos Eduardo Feliciano Medeiros | A definir |
| Carlos Eduardo Silva da Hora Anjos | A definir |
| Luciano Feitosa dos Santos | A definir |
| Carlos Ryan Pereira Castro | A definir |
| Ítalo Romão do Nascimento | A definir |
| Marco Antônio Macedo Santana | A definir |

> Preencham a coluna "Papel" (por exemplo, Scrum Master, Tech Lead, Desenvolvedor, QA).

## Tecnologia

- Android nativo, desenvolvido no **Android Studio**

## Como rodar o projeto

### Pré-requisitos

- [Android Studio](https://developer.android.com/studio) (versão estável mais recente)
- JDK 17 (já incluído no Android Studio)
- Um emulador Android configurado no AVD Manager **ou** um celular Android com depuração USB ativada
- Git

### Passo a passo

1. Clone o repositório:
   ```bash
   git clone https://github.com/<organizacao-ou-usuario>/projeto-integrado-mobile-corrige-ai.git
   cd projeto-integrado-mobile-corrige-ai
   ```
2. Troque para a branch de integração:
   ```bash
   git checkout develop
   ```
3. Abra o Android Studio, escolha **Open** e selecione a pasta do projeto Android dentro de `/src`.
4. Aguarde o **Gradle Sync** terminar.
5. Selecione um emulador ou dispositivo e clique em **Run ▶**.

> Observação: o código-fonte do app ficará em `/src`. Até lá, esta pasta contém apenas um arquivo `.keep`.

## Estrutura de pastas

| Caminho | Propósito |
|---|---|
| `/docs` | Documentação (wireframes, casos de uso, diagramas de arquitetura, regras de negócio, plano e casos de teste) |
| `/src` | Código-fonte principal do aplicativo |
| `/assets` | Recursos estáticos (ícones, logos, fontes, imagens, animações) |
| `/tests` | Testes unitários, de integração e de interface (UI) |
| `.github/` | Template de Pull Request e, futuramente, actions de CI/CD |

## Fluxo de trabalho (Git Flow simplificado)

- `main`: reflete o ambiente de produção; só recebe código testado e aprovado.
- `develop`: branch de integração, criada a partir da `main`.
- `feature/<nome>`, `docs/<nome>`, `fix/<nome>`: branches de trabalho criadas a partir da `develop`.

Regras:

1. Ninguém faz commit direto na `main` nem na `develop`.
2. Todo trabalho entra por **Pull Request**, com aprovação de pelo menos 1 outro integrante.
3. Versionamento por tags seguindo o [Versionamento Semântico](https://semver.org/lang/pt-BR/) (ex.: `v0.1.0-alpha`).

### Padrão de mensagens de commit

```
tipo: descrição curta no imperativo

feat: adiciona tela de login
docs: adiciona diagrama de classes
fix: corrige validação de senha
chore: atualiza .gitignore
test: adiciona caso de teste de cadastro
```
