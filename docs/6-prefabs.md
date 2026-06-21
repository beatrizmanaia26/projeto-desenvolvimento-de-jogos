# Prefabs

## **Visão Geral** <br>
Os prefabs (ou *prefabricated objects*) são componentes reutilizáveis do jogo que agrupam elementos visuais, físicos e lógicos em estruturas modulares. Em *O Enigma de Clarke*, os prefabs foram projetados para garantir consistência visual, facilitar a montagem dos cenários e padronizar o comportamento dos objetos interativos, inimigos e elementos do ambiente.

---

## **Categorias de Prefabs** <br>

### **1. Personagens** <br>

| Prefab | Descrição |
|--------|-----------|
| **Clarke (Protagonista)** | Personagem jogável com animações de andar, correr, pular, agachar, atacar e interagir. Possui sistema de vidas (5) e inventário. |
| **Lobo (Aliado)** | Acompanha Clarke em momentos narrativos. Possui animações de movimento e interação simbólica. |
| **Bruxa (Antagonista)** | Chefe final com animações de ataque, magia e derrota. Controla enigmas e obstáculos ao longo do jogo. |

---

### **2. NPCs (Personagens Não Jogáveis)** <br>

| Prefab | Descrição | Fase |
|--------|-----------|------|
| **Morador** | Introduz o contexto da vila abandonada. | Fase 1 |
| **Soldado Ferido** | Reforça o clima de decadência do reino. | Fase 1 |
| **Gnomo** | Apresenta o enigma da floresta e entrega um fragmento do pergaminho. | Fase 2 |
| **Pessoa na Moita** | Oferece pista para o enigma dos símbolos da entrada do castelo. | Fase 3 |
| **Bibliotecária** | Auxilia na progressão da fase com pistas e interações. | Fase 4 |
| **Fantasma do Rei** | Dá sentido ao enigma do trono amaldiçoado. | Fase 5 |
| **Mago** | Orienta a criação da poção final. | Fase 6 |
| **Aranha do Baú** | Revela informações sobre os segredos e tesouros do reino. | Fase 7 |

---

### **3. Inimigos** <br>

| Prefab | Descrição | Comportamento |
|--------|-----------|---------------|
| **Ratos** | Inimigos pequenos e rápidos. | Aparecem em áreas escuras; dificultam a movimentação. |
| **Guardas Reais** | Antigos protetores corrompidos pela bruxa. | Combate direto; ameaça maior. |
| **Criaturas Voadoras** | Inimigos ágeis que atacam pelo alto. | Exigem reflexos rápidos e atenção. |
| **Aranhas** | Surgem em regiões sombrias. | Reforçam a atmosfera de perigo. |

---

### **4. Obstáculos e Perigos do Cenário** <br>

| Prefab | Descrição |
|--------|-----------|
| **Espinhos** | Armadilhas que causam dano ao contato. |
| **Ácido Tóxico** | Área que impede a passagem; exige desvio ou pulo preciso. |
| **Plantas Perigosas** | Causam dano ao jogador. |
| **Elementos Móveis** | Objetos que podem ser movidos para alcançar áreas escondidas. |

---

### **5. Itens e Power-ups** <br>

| Prefab | Descrição | Função |
|--------|-----------|--------|
| **Moedas Antigas** | Colecionáveis espalhados pelo cenário. | Usadas na Fase 4 para progressão. |
| **Erva Luminosa** | Item de cura. | Recupera a vida de Clarke. |
| **Espada** | Item-chave. | Permite derrotar inimigos. |
| **Chave** | Item-chave. | Abre portas e caminhos trancados. |
| **Fragmentos do Pergaminho** | Itens de progressão. | Ajudam a resolver enigmas. |
| **Ingredientes da Poção** | Coletados na Fase 6. | Utilizados para criar a poção que enfraquece a bruxa. |
| **Símbolos Mágicos** | Colecionáveis escondidos. | Revelam informações sobre o mundo do jogo. |

---

### **6. Interações e Puzzles** <br>

| Prefab | Descrição |
|--------|-----------|
| **Objetos Interativos** | Itens que podem ser examinados, ativados ou coletados. |
| **Mecanismos** | Dispositivos que precisam ser ativados em ordem correta. |
| **Símbolos e Sequências** | Pistas visuais que devem ser interpretadas para resolver enigmas. |
| **Livros e Pergaminhos** | Elementos da Biblioteca Antiga que contêm pistas. |
| **Caldeirão** | Utilizado na Câmara das Poções Proibidas para preparar a poção final. |

---

### **7. Cenários** <br>

| Prefab | Descrição |
|--------|-----------|
| **Vila Abandonada** | Casas de madeira e ruínas. |
| **Floresta Sombria** | Árvores, sombras e elementos naturais. |
| **Entrada do Castelo** | Muralhas, portões e guardas. |
| **Biblioteca Antiga** | Estantes, livros e pergaminhos. |
| **Salão do Trono** | Trono, armaduras e símbolos mágicos. |
| **Câmara das Poções** | Frascos, ingredientes e caldeirão. |
| **Torre Final** | Última área com o confronto decisivo. |

---

### **8. Interface e HUD** <br>

| Prefab | Descrição |
|--------|-----------|
| **Inventário** | Sistema para armazenar e gerenciar itens coletados. |
| **HUD de Vidas** | Exibe as 5 vidas de Clarke. |
| **Menu Principal** | Tela inicial com opções de iniciar, continuar e configurações. |
| **Menu de Pausa** | Permite pausar o jogo e acessar opções. |
| **Indicadores de Progressão** | Mostram fragmentos coletados e fases concluídas. |

---

## **Estrutura de Implementação** <br>
Cada prefab será implementado com:

- **Sprite e animações**: para representação visual;
- **Colliders e Rigidbody**: para física e interação;
- **Scripts de comportamento**: para lógica específica (movimento, dano, coleta, etc.);
- **Sons e efeitos**: para feedback auditivo;
- **Sistema de pooling**: para otimização de performance (inimigos e itens).

---

## **Considerações Técnicas** <br>

- **Engine:** Unity (C#);
- **Resolução:** 1920x1080 (ajustável);
- **Controles:** Teclado (A/D, Shift, Espaço, Ctrl/C, E, I, Esc);
- **Perspectiva:** Side view 2D;
- **Build alvo:** PC (Windows).