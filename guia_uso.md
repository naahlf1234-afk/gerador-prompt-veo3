# 📖 Guia de Uso — Gerador de Prompt VEO3

## Como usar o system_prompt.md em cada plataforma

---

## 🤖 ChatGPT (Custom GPT)

1. Acesse chat.openai.com > Explorar GPTs > Criar GPT
2. Vá em "Configurar" > campo "Instruções"
3. Cole o conteúdo completo do `system_prompt.md`
4. Salve e teste seu GPT personalizado

---

## 💡 Claude (Anthropic) — Projects

1. Acesse claude.ai > Projetos > Criar novo projeto
2. Clique em "Instruções do projeto" ou "Custom instructions"
3. Cole o conteúdo do `system_prompt.md`
4. Todas as conversas naquele projeto usarão o prompt automático

---

## 💎 Google Gemini — Gems

1. Acesse gemini.google.com > Gems > Criar novo Gem
2. No campo "Instruções", cole o conteúdo do `system_prompt.md`
3. Dê um nome ao Gem e salve

---

## ⚡ API Direta (OpenAI, Anthropic, Groq...)

```python
import openai

# Leia o system prompt do arquivo
with open('system_prompt.md', 'r', encoding='utf-8') as f:
    system_prompt = f.read()

    client = openai.OpenAI(api_key='SUA_API_KEY')

    response = client.chat.completions.create(
        model='gpt-4o',
            messages=[
                    {"role": "system", "content": system_prompt},
                            {"role": "user", "content": "Cena de um astronauta sozinho na Lua olhando para a Terra"}
                                ]
                                )

                                print(response.choices[0].message.content)
                                ```

                                ---

                                ## 💡 Dicas de Uso

                                - **Ideia vaga?** O sistema vai perguntar os detalhes antes de gerar.
                                - **Ideia detalhada?** Mande direto e receba o prompt pronto.
                                - **Quer testar rápido?** Use: _"Cena de [personagem] em [lugar] fazendo [ação]"_
                                - **Quer fala no vídeo?** Inclua a frase desejada na sua descrição.
                                - **Sem fala?** Apenas diga que é uma cena silenciosa.
