# ache-a-diferente
# 🔍 Ache a Diferente!

Jogo de raciocínio visual em HTML/CSS/JS puro, single-file (`index.html`), pronto para hospedar no GitHub Pages.

## 🎮 Como jogar

- São exibidas **3 figurinhas** (emojis): **1 acima** e **2 abaixo**.
- **2 são iguais** e **1 é diferente**.
- Toque na figura **diferente** antes que o tempo acabe.

## 🏆 Pontuação e fases

- O jogo tem **20 fases**.
- Cada acerto vale **10 × número da fase** pontos (ex.: fase 5 = 50 pontos).
- Ao completar a fase 20, todas as figurinhas trocam (novo conjunto de emojis) e o jogo **recomeça da fase 1**, mantendo a pontuação.

## ❤️ Vidas (corações)

- Você começa com **3 vidas** (❤️❤️❤️).
- Cada erro (escolher a figura errada **ou** o tempo acabar) remove **1 vida** e:
  - **Repete a mesma fase**
  - **Reduz o tempo disponível em 25%** a cada erro consecutivo
- Ao perder **as 3 vidas**, é **Game Over**.
- Ao reiniciar, as vidas voltam a 3, mas o tempo volta ao normal da fase.

## ⏱️ Tempo por fase

- Fase 1: ~20 segundos
- Fase 20: ~10 segundos
- O tempo diminui linearmente conforme a fase avança.

## 🧩 Dificuldade progressiva

| Fases | Nível de diferença |
|-------|---------------------|
| 1–3   | Bem diferente (emojis totalmente distintos) |
| 4–6   | Ligeiramente diferente |
| 7–9   | Quase iguais, pouca diferença |
| 10–13 | Diferença muito sutil |
| 14–20 | Diferença mínima (máxima dificuldade) |

A "diferença sutil" é simulada com pequenas variações de **rotação, escala, opacidade e brilho** aplicadas na figurinha diferente — quanto maior a fase, menor a diferença visual.

## 🔁 Ciclo infinito

Ao completar as 20 fases, o jogo:
1. Mostra uma tela de parabéns
2. Troca o conjunto de figurinhas (animais → frutas → esportes → veículos → personagens...)
3. Recomeça da fase 1 com dificuldade crescente novamente

## 📱 PWA

O jogo inclui `manifest.json` e `sw.js` para funcionar como **Progressive Web App** (instalável e com cache offline).

> Obs.: adicione os ícones `icon-192.png` e `icon-512.png` na mesma pasta para a instalação completa do PWA.

## 📂 Arquivos

- `index.html` — jogo completo (HTML + CSS + JS)
- `manifest.json` — configuração PWA
- `sw.js` — service worker para cache offline

## 🚀 Deploy no GitHub Pages

1. Suba os arquivos para o repositório
2. Ative o GitHub Pages na branch principal
3. Acesse pelo link gerado (`https://seuusuario.github.io/seurepo/`)
4. © 2026 Michel Detilli.
Todos os direitos reservados. 
É permitido jogar online. É proibida a cópia, distribuição ou uso comercial do código sem autorização.
