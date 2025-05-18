# 📚 Assistente de Pesquisa Acadêmica com IA Gemini

Automatiza etapas-chave da sua pesquisa acadêmica com a API Google Gemini: da busca bibliográfica à formatação final.

**Última atualização:** 17/05/2025

---

## ⚙️ Funcionalidades

- **Instalação e Configuração**: Instala bibliotecas e configura a API Gemini automaticamente.
- **Interação com Gemini**: Permite perguntas diretas e busca de informações atualizadas.
- **Agentes Inteligentes (Funções):**
  1. **Busca Bibliográfica** – Encontra artigos relevantes.
  2. **Análise de Artigos** – Resume objetivos, métodos e conclusões.
  3. **Síntese da Literatura** – Gera um panorama claro e coeso.
  4. **Formatação** – Aplica estilo acadêmico (ex: ABNT, APA).
- **Saída em Markdown**: Resultados organizados e prontos para copiar diretamente no Colab.

---

## 🧩 Requisitos

- Conta Google com acesso ao Colab.
- Chave da API Gemini (crie em [Google AI Studio](https://aistudio.google.com/app/apikey)).

---

## 🚀 Como Usar

1. **Abra no Colab**: Faça upload do `.ipynb` ou cole o código.
2. **Configure a API**:
   - Clique no ícone 🔑 "Secrets" no Colab.
   - Adicione `GOOGLE_API_KEY` com sua chave da API.
3. **Instale as bibliotecas**:
   ```python
   %pip install -q google-generativeai pillow requests
   ```
4. **Execute o script principal**:
   - Digite o tópico da pesquisa quando solicitado.
   - Acompanhe cada etapa (busca → análise → síntese → formatação).
   - (Opcional) Escolha o formato final de saída: ex: “artigo” "entrevista" ou deixe em branco e tecle Enter.

---

## 🧠 Estrutura do Código

| Agente                       | Função                                |
|------------------------------|---------------------------------------|
| `agente_busca_bibliografica` | Localiza artigos e links              |
| `agente_analise_artigos`     | Resume o conteúdo dos artigos         |
| `agente_sintese_literatura`  | Cria uma revisão integrada            |
| `agente_formatacao`          | Aplica normas acadêmicas              |
| `agente_saida_usuario`       | Exibe os resultados no Colab          |

---

## 🔍 Observações Importantes

- **Qualidade** depende da clareza dos prompts e capacidades do modelo.
- **Limites de uso**: verifique cotas e preços da [API Gemini](https://ai.google.dev/pricing).
- **Busca não é exaustiva** – recomenda-se uso complementar de bases acadêmicas.
- **Código testado em mai/2025** – atualizações podem ser necessárias com o tempo.

---

## 💡 Melhorias Futuras

- Integração com Google ADK (estrutura modular de agentes).
- Exportação para `.md`, `.txt` , etc.
- Interface com Gradio ou Streamlit.
- Cache para evitar chamadas repetidas à API.

---

## 📄 Licença

Código aberto. Modifique, use e compartilhe livremente. Recomendamos adicionar uma licença oficial como a [MIT License](https://opensource.org/licenses/MIT).
