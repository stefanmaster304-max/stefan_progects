===============================================================================
THE CONFRONT - LEIA-ME / README (Versão 0.1)
===============================================================================

Bem-vindo ao The Confront, um jogo de ação tática em áudio 3D desenvolvido no motor NVGT com integração avançada de King Audio Engine e FMOD.

-------------------------------------------------------------------------------
1. VISÃO GERAL E OBJETIVO
-------------------------------------------------------------------------------
The Confront coloca o jogador em cenários e arenas dinâmicas com combate em tempo real contra diversos tipos de NPCs armados e perigosos. O jogo foi desenhado especificamente com áudio espacial 3D imersivo e acessibilidade total para jogadores com deficiência visual, incluindo suporte nativo a leitores de tela e áudio posicional HRTF.

-------------------------------------------------------------------------------
2. CONTROLES BÁSICOS
-------------------------------------------------------------------------------
- Setas Direcionais (Cima, Baixo, Esquerda, Direita): Movimentação do personagem no plano 2D (Norte, Sul, Leste, Oeste). A velocidade de deslocamento é determinada pelos atributos do personagem selecionado.
- Q / E: Girar orientação e mira do personagem (Q gira à esquerda, E gira à direita em incrementos de 45 graus: Norte, Nordeste, Leste, Sudeste, Sul, Sudoeste, Oeste, Noroeste).
- Barra de Espaço: Pular / Saltar.
- S: Alternar postura (Sentar / Levantar).
- Page Up / Page Down: Subir ou descer escadas quando em uma casa de escada.
- Left Control (Ctrl Esquerdo): Disparar arma equipada.
  * Nota de combate: Apenas o Control Esquerdo dispara a arma.
- R: Recarregar arma equipada utilizando a munição reserva compatível.
- Enter: Interagir com itens no chão, portas e objetos.
- I: Abrir inventário do jogador.
- W: Ciclar armas equipadas / inventário de armas.
- H: Anunciar vida e status atual.
- Alt + Setas: Ajustar volumes de áudio e música.
- Escape: Pausar, voltar em menus ou fechar diálogos.

-------------------------------------------------------------------------------
3. PERSONAGENS JOGÁVEIS (STEFAN & ILANA)
-------------------------------------------------------------------------------
No menu de Opções, na opção "Selecione o seu personagem", você pode escolher o seu protagonista. Pressione a Barra de Espaço em cima de cada um para ouvir sua descrição completa:

- Stefan (Masculino):
  * O garoto rebelde de corpo atlético, sarado, cabelo loiro e barba longa, segurando uma metralhadora de dois canos nas mãos.
  * Vida máxima base: 5.000 HP.
  * Movimentação: 5% mais lenta do que a velocidade padrão.
  * Sons de dor em combate: Voz própria masculina exclusiva de Tristan (vozes 1 a 16).
  * Sons de morte: Sequência de morte com Tristan voz 17 combinada aos efeitos de impacto e queda (misc331, misc333, misc334).

- Ilana (Feminino):
  * Uma garota de corpo atlético, sarado e bem atraente, cabelo loiro longo, segurando um rifle de dois longos canos de cor dourada que brilha no escuro.
  * Vida máxima base: 10.000 HP.
  * Movimentação: 5% mais rápida do que a velocidade padrão.
  * Sons de dor em combate: Voz própria feminina exclusiva de Aria (vozes 1 a 16).
  * Sons de morte: Sequência de morte com Aria voz 17 combinada aos efeitos de impacto e queda (misc331, misc333, misc334).

Observações:
- Os efeitos sonoros gerais de passos, saltos, aterrissagens, interface e equipamentos são universais e compartilhados entre ambos.
- A seleção de personagem é salva de forma persistente tanto nas configurações gerais quanto no arquivo de progresso do jogo.

-------------------------------------------------------------------------------
4. SISTEMA DE COMBATE E ARMAS
-------------------------------------------------------------------------------
- O arsenal conta com 80 armas categorizadas em rifles, metralhadoras, pistolas, revólveres, escopetas, rifles de precisão, lançadores e combate corpo a corpo.
- Balística e Projéteis em Tempo Real: Cada disparo gera um projétil ativo simulado em 3D (balístico, foguete, granada ou feixe de energia laser).
- Paredes e Obstáculos: Disparos não atravessam paredes sólidas. Disparos contra alvos alinhados em direções cardeais causam dano real aos inimigos.
- Cada arma possui seu dispositivo de alimentação (carregador, câmara, cilindro ou tubo) e consome munições específicas presentes no inventário.

-------------------------------------------------------------------------------
5. INIMIGOS E NPCS
-------------------------------------------------------------------------------
- Os mapas contam com geradores de NPCs dinâmicos com zonas de patrulha e limites de perseguição definidos.
- Os NPCs possuem inteligência artificial tática com desvio de obstáculos, patrulha perimetral, vocalizações 3D e combate posicional.
- Ao serem eliminados, os NPCs podem deixar cair itens de valor, munições e moedas.

-------------------------------------------------------------------------------
6. LOJA E ECONOMIA
-------------------------------------------------------------------------------
- O menu da loja é organizado em prateleiras e categorias temáticas.
- A economia suporta múltiplas moedas nativas: Ouro, Prata, Diamante e Cristal Dourado.
- Os itens adquiridos são enviados diretamente para o inventário do personagem.

-------------------------------------------------------------------------------
7. MAPAS E PROGRESSÃO
-------------------------------------------------------------------------------
- Acesso ao "Menu de mapas" no menu principal para visualizar e definir o seu mapa padrão entre os mapas já desbloqueados.
- Ao clicar em "Jogar", o jogo carrega diretamente o mapa selecionado.
- A progressão do jogador salva automaticamente nível, experiência, ressurreições, personagem e inventário.

-------------------------------------------------------------------------------
8. AJUDA E DOCUMENTAÇÃO
-------------------------------------------------------------------------------
- No menu principal, a opção "Ajuda" permite ler o histórico de alterações recentes e este guia completo sem sair do jogo, em um editor multilinha interativo.
- Pressione Escape a qualquer momento no visualizador para fechar o texto e retornar ao menu.
