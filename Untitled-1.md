<h3><u>SCHEMA DE LA CHAINE DE COMPILATION ET DE CHARGEMENT DE PROGRAMME EN MEMOIRE</u></h3>

```
                               CODE SOURCE
                             (programme.cpp)
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │    PRÉPROCESSEUR    │ ← prépare le code
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