# dados55

Repositório para Edge Functions do Supabase, incluindo a função `process-document` que processa documentos usando OpenAI GPT-4.

## Estrutura

```
supabase/
  └── functions/
      └── process-document/
          └── index.ts      # Implementação da Edge Function
```

## Edge Functions

### process-document

Função responsável por processar documentos usando o modelo GPT-4o-2024-11-20 da OpenAI. A função:

1. Recebe o texto do documento
2. Processa usando o prompt específico
3. Retorna uma estrutura JSON com:
   - Metadados do documento
   - Conteúdo estruturado
   - Relacionamentos
   - Tags

## Configuração

A função requer as seguintes variáveis de ambiente:
- OPENAI_API_KEY
- SUPABASE_URL
- SUPABASE_ANON_KEY
