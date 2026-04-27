# 🎬 Gerador de Prompt VEO3

> Sistema completo de geração de prompts cinematográficos de alto nível para o Google VEO3.
>
> ---
>
> ## 📌 O que é isso?
>
> Este repositório contém um **system prompt completo** para transformar qualquer ideia em um prompt profissional para o Google VEO3 — a IA de geração de vídeo do Google.
>
> A lógica é baseada em conceitos públicos de direção cinematográfica aplicados à engenharia de prompts para IA generativa de vídeo.
>
> ---
>
> ## 🗂️ Estrutura do Repositório
>
> ```
> gerador-prompt-veo3/
> │
> ├── README.md                  # Este arquivo
> ├── system_prompt.md           # O system prompt completo
> ├── guia_uso.md                # Como usar em ChatGPT, Claude, Gemini
> └── exemplos/
>     ├── exemplo_urbano.md
>     ├── exemplo_natureza.md
>     └── exemplo_drama.md
> ```
>
> ---
>
> ## 🧠 Como Funciona
>
> O sistema atua como um **diretor de cinema + especialista em IA**, seguindo 7 etapas:
>
> 1. **Entendimento da ideia** — extrai tema, emoção e objetivo
> 2. 2. **Construção da cena** — estrutura ambiente, personagem, ação e ritmo
>    3. 3. **Direção cinematográfica** — define câmera, iluminação e estilo visual
>       4. 4. **Design sensorial** — adiciona sons, efeitos e texturas
>          5. 5. **Fala** (opcional) — define voz, sotaque e tom emocional em português
>             6. 6. **Tradução para IA** — converte tudo em inglês técnico e descritivo
>                7. 7. **Output estruturado** — entrega sempre em 3 partes obrigatórias
>                  
>                   8. ---
>                  
>                   9. ## 📤 Formato de Output
>                  
>                   10. ### 🎦 1. Prompt Cinematográfico
>
> Parágrafo único em **inglês**, altamente descritivo, otimizado para geração visual realista no VEO3.
>
> ### ⚙️ 2. Prompt Técnico em JSON
>
> ```json
> {
>   "description": "...",
>   "style": "cinematic, ultra realistic",
>   "camera": "slow push-in, slight handheld movement",
>   "lighting": "dramatic high contrast, neon tones",
>   "environment": "...",
>   "elements": ["...", "..."],
>   "motion": "...",
>   "ending": "...",
>   "voice": {
>     "text": "...",
>     "language": "pt-BR",
>     "gender": "...",
>     "age": "...",
>     "accent": "...",
>     "tone": "..."
>   },
>   "text": "none",
>   "keywords": ["cinematic", "no subtitles"]
> }
> ```
>
> ### 🖼️ 3. Prompt de Imagem (Frame 1)
>
> Prompt otimizado para gerar a imagem do primeiro frame no Midjourney, DALL-E ou Stable Diffusion.
>
> ---
>
> ## ⚙️ Como Usar
>
> 1. Abra o arquivo `system_prompt.md`
> 2. 2. Copie o conteúdo completo
>    3. 3. Cole como **System Prompt** em qualquer LLM (ChatGPT, Claude, Gemini, etc.)
>       4. 4. Mande sua ideia e receba o prompt completo em 3 partes
>         
>          5. ---
>         
>          6. ## 📋 Regras do Sistema
>         
>          7. - ✅ Prompt principal sempre em **inglês**
> - ✅ Fala (se houver) sempre em **português**
> - - ✅ Sempre incluir **"no subtitles"**
>   - - ✅ Duração alvo: **~8 segundos**
>     - - ✅ Output sempre com as **3 partes obrigatórias**
>       - - ❌ Nunca entregar resultado incompleto
>         - - ❌ Nunca fazer descrições vagas ou genéricas
>          
>           - ---
>
> ## 🚀 Uso Recomendado
>
> | Plataforma | Como usar |
> |-----------|-----------|
> | ChatGPT | Custom GPT ou System Prompt via API |
> | Claude | System Prompt no Project |
> | Gemini | Instructions no Gem |
> | API direta | Campo `system` da requisição |
>
> ---
>
> ## 📄 Licença
>
> Uso pessoal. Técnicas de prompt engineering para VEO3 são de domínio público.
