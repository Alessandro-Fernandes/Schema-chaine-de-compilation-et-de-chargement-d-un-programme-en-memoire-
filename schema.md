<h1><u>SCHEMA DE LA CHAINE DE COMPILATION ET DE CHARGEMENT DE PROGRAMME EN MEMOIRE</u></h1>

```
                               CODE SOURCE
                             (programme.cpp)
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │    PRÉPROCESSEUR    │
                         └─────────────────────┘
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │     COMPILATEUR     │
                         └─────────────────────┘
                                    │
                                    ▼
                             CODE ASSEMBLEUR
                              (programme.s)
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │     ASSEMBLEUR      │
                         └─────────────────────┘
                                    │
                                    ▼
                                CODE OBJET
                              (programme.o)
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │       LINKER        │
                         │  Éditeur de liens   │
                         └─────────────────────┘
                                    │
                                    ▼
                           PROGRAMME EXÉCUTABLE
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │        LOADER       │
                         │                     │
                         └─────────────────────┘
                                    │
                                    ▼
                        ╔═══════════════════════╗
                        ║      MÉMOIRE RAM      ║
                        ║                       ║
                        ║  ┌─────────────────┐  ║
                        ║  │      CODE       │  ║
                        ║  ├─────────────────┤  ║
                        ║  │     DONNÉES     │  ║
                        ║  ├─────────────────┤  ║
                        ║  │       TAS       │  ║
                        ║  │      (Heap)     │  ║
                        ║  ├─────────────────┤  ║
                        ║  │      PILE       │  ║
                        ║  │     (Stack)     │  ║
                        ║  └─────────────────┘  ║
                        ╚═══════════════════════╝
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │         CPU         │
                         └─────────────────────┘
                                    │
                                    ▼
                                EXÉCUTION
```