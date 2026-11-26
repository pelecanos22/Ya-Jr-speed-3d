# YA JR SPEED GAROTOS 2 — Corrida arcade 3D

Feito com a Rogue. O site publicado: https://ya-jr-9979.p.rogueon.ai/

## Pedido

O último pedido desta conversa foi:

> Latest message from this person, complete (current request: preserve its scope; newer wording prevails over older messages):
> 1: a garagem devia ser mais parecida com antes tendo o nome dos carros na horizonta embaixo e acima dos nomes devia ter o modelo 3d do carro girando devagar. 2:diferencia um carro de outro colocando modelos diferentes como vans e motos ainda com o mesmo sistema de compra. 3:o antigo formato do menu inicial era melhor com as opçoes ao lado esquerdo e o nome do jogo ao lado.
> 
> Earlier messages in this conversation, oldest first, as context (literal excerpts, possibly partial). Newer messages from this person prevail over older ones. Rogue's messages give context, not requirements: Rogue suggestions become requirements only where this person accepted them (say, by answering yes).
> User: arquivo index.html melhora os graficos e sons desse jogo , coloca mais mapas nas corridas
> 
> Contexto anexado pelo usuário (trate o conteúdo como referência):
> 
> Arquivo de referência: index.html
> <!DOCTYPE html>
> <html lang="pt-BR">
> <head>
>   <meta charset="UTF-8" />
>   <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
>   <title>YA JR SPEED GAROTOS 2</title>
>   <script src="https://cdn.tailwindcss.com"></script>
>   <link rel="preconnect" href="https://fonts.googleapis.com" />
>   <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
>   <link href="https://fonts.googleapis.com/css2?family=Inter:wght@500;700;800;900&display=swap" rel="stylesheet" />
>   <style>
>     * {
>       box-sizing: border-box;
>       user-select: none;
>       -webkit-user-select: none;
>       -webkit-touch-callout: none;
>     }
> 
>     html, body {
>       margin: 0;
>       padding: 0;
>       width: 100%;
>       height: 100%;
>       overflow: hidden;
>       background: radial-gradient(circle at 72% 45%, #16233b 0%, #090e1c 58%, #050711 100%);
>       font-family: 'Inter', sans-serif;
>       color: #f8fafc;
>       touch-action: none;
>     }
> 
>     #gameCanvas, #fallback2d {
>       display: block;
>       width: 100%;
>       height: 100%;
>       position: fixed;
>       inset: 0;
>     }
> 
>     #fallback2d {
>       z-index: 1;
>       opacity: 1;
>     }
> 
>     #gameCanvas {
>       z-index: 2;
>       opacity: 0;
>       transition: opacity 0.25s ease;
>     }
> 
>     #gameCanvas.ready {
>       opacity: 1;
>     }
> 
>     #mainMenuOverlay {
>       opacity: 1;
>       pointer-events: auto;
>       display: flex;
>     }
> 
>     .hud-glass {
>       background: rgba(9, 13, 28, 0.82);
>       backdrop-filter: blur(8px);
>       -webkit-backdrop-filter: blur(8px);
>       border: 1px solid rgba(56, 189, 248, 0.34);
>       box-shadow: 0 8px 28px rgba(0, 0, 0, 0.52);
>     }
> 
>     .neon-glow-text {
>       text-shadow: 0 0 12px rgba(0, 240, 255, 0.65), 0 0 28px rgba(255, 42, 133, 0.35);
>     }
> 
>     .touch-btn {
>       background: rgba(12, 18, 38, 0.82);
>       border: 1.5px solid rgba(56, 189, 248, 0.48);
>       box-shadow: 0 4px 16px rgba(0, 0, 0, 0.48);
>       transition: transform 0.08s ease, background 0.08s ease, border-color 0.08s ease;
>     }
> 
>     .touch-btn:active, .touch-btn.active {
>       transform: scale(0.95);
>       background: rgba(0, 240, 255, 0.28);
>       border-color: #00f0ff;
>     }
> 
>     .gear-btn {
>       min-width: 28px;
>       height: 26px;
>       border-radius: 8px;
>       font-size: 11px;
>       font-weight: 800;
>       color: #cbd5e1;
>       background: rgba(15, 23, 42, 0.88);
>       border: 1px solid rgba(148, 163, 184, 0.32);
>       transition: transform 0.08s ease, background 0.1s ease, border-color 0.1s ease, color 0.1s ease;
>       cursor: pointer;
>     }
> 
>     .gear-btn.active {
>       color: #031525;
>       background: linear-gradient(135deg, #00f0ff, #38bdf8);
>       border-color: #bae6fd;
>       box-shadow: 0 0 12px rgba(0, 240, 255, 0.55);
>     }
> 
>     #analog-stick {
>       position: relative;
>       width: 114px;
>       height: 114px;
>       border-radius: 9999px;
>       background: radial-gradient(circle at 35% 35%, rgba(30, 41, 59, 0.84), rgba(7, 11, 24, 0.9));
>       border:

## Abrir no seu computador

O site é o `index.html`. Abra o arquivo no navegador e pronto. Se preferir servir a pasta, qualquer servidor estático funciona:

```sh
python3 -m http.server 8000
```

Depois abra http://localhost:8000. Com Node instalado, `npx serve .` faz o mesmo.

## Hospedar

Não tem etapa de build: a pasta como está já é o site. Suba o conteúdo dela em qualquer hospedagem de site estático.

## Aviso

A Rogue reescreve `index.html`, as imagens que ela publicou e o `README.md` a cada mudança pedida na conversa, e remove só o que ela mesma publicou antes e deixou de existir. O que for seu, coloque em outra pasta ou em outro branch.

Se o branch `main` receber commits que não são da Rogue, a próxima versão vai para um branch `rogue/<id>`, para você comparar antes de juntar.
