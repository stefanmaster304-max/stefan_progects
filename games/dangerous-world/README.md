# Dangerous World!

Código-fonte do jogo **Dangerous World!**, atualizado para NVGT 0.90.0-dev. Este diretório reúne o código e os dados de configuração versionáveis.

## Áudio

No alvo Windows, a espacialização usa King Audio com HRTF global ativo. Os rumos são enviados em graus, no padrão documentado pelo King Audio. O helper do pool é baseado no material da skill NVGT e mantém sons ambientes em 2D estacionário, pausando-os e retomando-os quando o jogador sai e volta à área. As bibliotecas King Audio, FMOD e Phonon usadas no alvo Windows ficam em `lib/`.

O material King Audio incluído na skill contém DLLs para Windows; não inclui uma biblioteca King Audio para Linux. O backend King Audio desta versão depende, portanto, do alvo Windows. A compilação Linux ainda precisa de um backend compatível com esse plugin para produzir uma build equivalente.

O jogo carrega os sons diretamente das subpastas categorizadas de `sounds/` (por exemplo, `sounds/player/`, `sounds/weapons/`, `sounds/map platforms/`, `sounds/Musics/` e `sounds/anbients/`). O pacote de áudio não está incluído neste repositório; coloque a pasta `sounds/` fornecida com o jogo ao lado de `dw.nvgt` ou do executável. O código não exige que os sons sejam reunidos em um arquivo único.

## Dados locais

Preferências e progresso ficam no diretório de dados do usuário informado pelo NVGT, dentro de `StefanGames/Dangerous World`. As opções são gravadas em `settings.dat`; os dados do jogador — mapa e posição atuais, nível, experiência, eliminações, saúde, inventário, arma equipada, escudo e mapas descobertos — ficam em `game_save.dat`. O jogo cria o arquivo de preferências com os valores padrão na primeira execução e salva o progresso automaticamente durante a partida.

## Sistemas retirados

Foram removidos os sistemas de fome e sede, coleta de recursos do piso, mãos esquerda/direita, NPCs, calendário e mensagens diárias. Itens no chão são recolhidos automaticamente quando o jogador se aproxima. O inventário rápido percorre os itens com Tab e Shift+Tab; Espaço pula, Alt+Enter interage com portas e pontos de viagem, e Enter abre lojas próximas.

## Atualizações

O menu principal consulta por HTTP os releases do repositório `stefanmaster304-max/stefan_progects` usando a API oficial do GitHub. Se houver um release, o jogo informa a versão e copia o endereço da página de releases para a área de transferência. No momento, o repositório ainda não tem release publicado.

## Compilação

Para compilar o alvo Windows, use NVGT 0.90.0-dev e deixe as DLLs King Audio e FMOD de `lib/` disponíveis na pasta de plugins do compilador e junto ao executável:

```text
nvgt -p windows -c dw.nvgt
```

O compilador Linux NVGT 0.90.0-dev foi instalado neste ambiente. O instalador Windows foi baixado do release oficial, mas o Wine deste ambiente encerrou a instalação com `Bad system call`; a compilação final Windows ainda precisa ser confirmada em uma instalação funcional do compilador Windows.
