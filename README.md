# ULS+ (ULSPLUS)

Aplicação Android para **idosos utentes da ULS** (Unidade Local de Saúde), pensada para ajudar no dia a dia da sua saúde, com foco em **acessibilidade**: texto grande, alto contraste, botões grandes e opção «Ouvir» nas informações importantes.

Projeto académico — **Grupo 11**.

## Funcionalidades principais

A aplicação está organizada em quatro separadores:

- **Medicação** (ecrã inicial) — próxima toma, adicionar medicamentos e lembretes.
- **Aprender** — informação útil (cirurgia, alta, evitar quedas), quizzes e prémios.
- **Segurança** — conselhos e prevenção.
- **Ajuda** — botão «Preciso de ajuda» e contactos.

Inclui ainda contas de utilizador (criar conta / entrar) e informação sobre como marcar e desmarcar consultas.

## Tecnologias

- Kotlin
- Jetpack Compose + Material 3
- Gradle (Kotlin DSL) com version catalog (`libs.versions.toml`)
- minSdk 24

## Estrutura do repositório

```
ULSPLUS/
├── docs/                         # Documentação do projeto
│   ├── Diagramas_G11/            # Diagramas (casos de uso, classes, sequência, estados, BPMN...)
│   ├── Proposta_de_Sistema_G11.docx
│   └── Prompts_Figma_G11.md      # Especificação dos ecrãs (design)
└── src/                          # Projeto Android Studio
    ├── app/
    │   ├── build.gradle.kts
    │   └── src/
    │       ├── main/
    │       │   ├── AndroidManifest.xml
    │       │   ├── java/upca/example/healthsolutions/ulsplus/
    │       │   │   ├── MainActivity.kt
    │       │   │   └── ui/theme/         # Cores, tipografia e tema Compose
    │       │   └── res/                  # Recursos (strings, ícones, temas)
    │       ├── test/                     # Testes unitários
    │       └── androidTest/              # Testes instrumentados
    ├── gradle/                   # Wrapper e catálogo de versões
    ├── build.gradle.kts
    └── settings.gradle.kts
```

## Como executar

1. Abrir a pasta **`src/`** no Android Studio.
2. Aguardar a sincronização do Gradle.
3. Executar a configuração `app` num emulador ou dispositivo.

Ou pela linha de comandos (dentro de `src/`):

```bash
./gradlew assembleDebug
```
