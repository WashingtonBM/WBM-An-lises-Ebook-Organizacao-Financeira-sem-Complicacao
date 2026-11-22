# WBM — Organização Financeira sem Complicação

Ebook interativo de educação financeira pessoal em página única, com planilhas editáveis, calculadoras, exercícios, gerador de plano e o consultor virtual Dáblio. [https://wbm-c79a.p.rogueon.ai/]

## Conteúdo do ebook

- 11 capítulos: introdução ao método WBM, diagnóstico financeiro, orçamento, reserva de emergência, dívidas, metas, hábitos, primeiros passos nos investimentos, exercícios, plano personalizado e referências.
- Raio-X financeiro, calculadora de reserva, planilha de orçamento mensal, planilha de dívidas com simulador de quitação (avalanche e bola de neve), cadastro de metas, checklist de hábitos e quiz de seis perguntas com correção.
- Gerador de plano personalizado com download em arquivo .txt e progresso de leitura com 12 itens no sumário.
- Dáblio: consultor virtual que responde apenas com base no conteúdo interno do ebook, após uma espera de 10 segundos.

## Estrutura do repositório

```text
index.html
README.md
public/rogue-images/c6b1fb11-5fa9-4534-a752-bf5901e1ce7f.webp
```

- index.html: a página completa. Todo o CSS e o JavaScript estão embutidos, sem dependências externas, fontes ou bibliotecas.
- public/rogue-images/: capa do ebook, usada no menu lateral e na capa. Mantenha o mesmo caminho relativo usado no HTML.

## Publicar no GitHub Pages

1. Crie o repositório ou use um existente e envie index.html, README.md e a pasta public/.
2. Em Settings, abra Pages e selecione Deploy from a branch.
3. Escolha a branch main e a pasta raiz (/).
4. O endereço público fica em https:[(https://github.com/WashingtonBM/WBM-An-lises-Ebook-Organizacao-Financeira-sem-Complicacao/edit/main/README.md)]

## Rodar localmente

Abra o arquivo index.html no navegador para ler, preencher as planilhas e gerar o plano. O Dáblio depende do proxy /__api/openrouter do ambiente da Rogue, então fora dele o chat informa que o serviço não está disponível.

## Dados e privacidade

- Tudo o que o leitor preenche fica no localStorage do navegador, na chave wbm.ofsc.v1: orçamento, dívidas, metas, hábitos e capítulos concluídos.
- Não existe conta de usuário nem banco de dados do ebook. A única informação enviada a terceiros é a pergunta feita ao Dáblio.
- Limpar os dados do navegador apaga as informações salvas. Use os botões de download (CSV do orçamento, CSV das dívidas e plano em .txt) para guardar cópias.

## Dáblio e chave de API

- As respostas usam a API da OpenRouter por meio do proxy da Rogue. A chave fica no estúdio da Rogue e nunca no HTML ou no repositório.
- Sem chave conectada, o chat avisa que falta configuração e mostra o trecho do ebook relacionado à pergunta.
- Perguntas fora do escopo financeiro recebem uma resposta padronizada; perguntas financeiras sem resposta no material também são sinalizadas, com convite a outra pergunta.

## Acessibilidade

- Imagens com texto alternativo, rótulos em todos os campos, foco visível, marcos de navegação e regiões com aria-live nos resultados.
- Layout responsivo de telas pequenas a monitores amplos, com menu lateral recolhível no celular e respeito a prefers-reduced-motion.

## Aviso

Conteúdo educacional. Não constitui recomendação de investimento.
