# Game Design Document

## 1. Overview
O Project X é um jogo ...

----------------
## 2. Mecânicas Principais (Gameplay)


--------------------
## 3. História e Lore

-------------------
## 4. Referências

## 5. Opções de Temas

O tema ainda será definido, mas aqui estão algumas opções para orientar o desenvolvimento:

* Dark Fantasy: Um mundo sombrio onde facções mágicas e biológicas lutam pelo controle, inspirando-se na Companhia Negra.
* Distopia Tecnológica: Facções de capitalismo corporativo versus socialismo tecnológico lutam pelo controle de recursos em um futuro pós-apocalíptico.
* Mix de Magia e Mecânica: Um universo onde facções misturam magia e tecnologia para construir máquinas de guerra e criaturas biológicas, como no Leviatã de Thomas Hobbes.
* Ficção Científica no Espaço: Facções de colônias espaciais com sistemas políticos divergentes (capitalismo galáctico versus comunas espaciais) lutam pelo controle de planetas ricos em recursos.
* Steampunk vs. Biotecnologia: Facções com máquinas a vapor avançadas enfrentam facções que utilizam criaturas biológicas modificadas geneticamente.
-------------------

## 6. Design Patterns e Arquitetura

### 6.1. Máquina de Estados (State Pattern)
* **Estado do jogo:** Controla os principais estados como Menu, Jogo, Pause, Game Over.
* **Modos de jogo:** Define o comportamento específico dos modos (Sobrevivência, Campanha).
* **IA dos Inimigos:** Utiliza estados como "Patrulhar", "Atacar", "Congelar", com transições dinâmicas baseadas nas condições do jogo.
### 6.2. Singleton Pattern
* **GameManager:** Controla o fluxo principal do jogo, garantindo que uma única instância esteja gerenciando os estados do jogo.

### 6.3. Factory Pattern

* Usado para a criação de inimigos e defesas, permitindo uma fácil expansão das variações de torres e tipos de inimigos.
