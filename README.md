# App NBA – Boston Celtics (Team Manager)

Aplicação Android para gerir o plantel dos Boston Celtics. Projeto do 1.º ano do CTeSP em Desenvolvimento para Dispositivos Móveis, no ISTEC Lisboa.

## Funcionalidades
- Lista de jogadores ordenada pelo número da camisola, com contador de jogadores
- Adicionar e editar jogadores: nome, posição, número e idade
- Foto do jogador, tirada com a câmara ou escolhida da galeria
- Ecrã de detalhe de cada jogador
- Remover jogadores, com confirmação (pressão longa na lista ou botão no detalhe)
- Validação de dados, incluindo números de camisola repetidos
- Dados guardados localmente em SQLite

## Tecnologias
- Java e Android SDK
- SQLite (`SQLiteOpenHelper`)
- RecyclerView, Material Components, CardView e ConstraintLayout
- CircleImageView

## Estrutura
```
app/src/main/java/com/example/teammanager/
├── activities/   # MainActivity, AddEditPlayerActivity, PlayerDetailActivity
├── adapters/     # PlayerAdapter
├── database/     # DatabaseHelper (SQLite)
└── models/       # Player
```

## Como correr
1. Abre a pasta do projeto no **Android Studio**.
2. Espera que o Gradle sincronize.
3. Corre a app num emulador ou telemóvel com **Android 16 (API 36)**, a versão mínima definida em `app/build.gradle`.
