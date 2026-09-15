# E-mails Réveillon 2026/2027 — Pousada Jardim Monte Verde

Notas de entrega dos 6 e-mails (2 fluxos), a partir do briefing `Briefing_Emails_Reveillon_Pousada_Jardim_Monte_Verde.docx.pdf` + feedback da equipe.

## Arquivos desta entrega

Pasta `emails/`:

- 6 arquivos `fluxoX-eY-nome.html` → cola no editor de HTML do e-mail no RD Station (o código completo do e-mail, já com as imagens apontando pro GitHub).
- 6 arquivos `fluxoX-eY-nome-preview.html` → prévia standalone (imagens embutidas no próprio arquivo), abre direto no navegador sem precisar subir nada antes. Não vai pro RD, é só pra você conferir.
- `imagens/` → os 6 banners novos (`email-banner-*.jpg`). Confirmado: fica no repositório `emails-jardim` mesmo, subindo a pasta `emails/` completa, do jeito que você já faz. Os 6 HTMLs de produção apontam pra `https://raw.githubusercontent.com/giuiia/emails-jardim/main/emails/imagens/email-banner-*.jpg` (o caminho com `emails/` aninhado dentro do repositório, que é onde o conteúdo cai quando a pasta inteira é enviada). **Conferi agora e as 6 imagens estão no ar nesse caminho.**

## Feedback incorporado

1. **Banners bem mais baixos**: 600×260 (proporção bem mais horizontal que o padrão anterior), pra caber tudo sem precisar rolar a tela.
2. **Foto + texto sobreposto em todos os 6 banners**: logo (menor e branco, direto sobre a foto, sem cabeçalho verde atrás) + selo "RÉVEILLON 2026/2027" + frase de destaque, com gradiente escuro sutil no topo (pro logo) e mais forte embaixo (pro texto), garantindo leitura em qualquer foto.
3. **Texto do desconto/oferta visível assim que abre**: logo abaixo do banner tem uma barra em âmbar com o texto da oferta (em texto de verdade, não dentro da imagem) — aparece mesmo que o cliente de e-mail bloqueie imagem por padrão (bem comum no Outlook e no Gmail).
4. **Textos centralizados**: todo o corpo do e-mail (parágrafos, frase de fechamento, botões) ficou centralizado, com uma exceção proposital: o depoimento da hóspede no e-mail de prova social (Fluxo 1 · E2) continua alinhado à esquerda, no estilo citação com a linha vertical.
5. **Sem link de cancelar inscrição**: removi essa linha do rodapé de todos os 6 e-mails, como pedido. Vale só um alerta rápido: dependendo da configuração do RD Station e da legislação de e-mail marketing, a própria plataforma pode inserir automaticamente uma opção de descadastro no envio, independente do que está no nosso HTML, isso não é algo que eu controle por aqui.

## Como colar no RD Station

O e-mail é diferente da LP: não é a técnica de injeção com `#jmv-lp`, é só colar o HTML completo no editor de e-mail do RD (opção de importar/editar HTML na automação ou no disparo de e-mail). Assunto e preview text são campos separados na tela de configuração do e-mail, não fazem parte do HTML:

| E-mail | Assunto | Preview text |
|---|---|---|
| Fluxo 1 · E1 | Seu Réveillon na Pousada Jardim começa aqui ✨ | Você acabou de dar o primeiro passo para viver uma virada de ano diferente. |
| Fluxo 1 · E2 | O que os hóspedes mais comentam sobre a Pousada Jardim | 4,5 no TripAdvisor. E olha o que uma hóspede contou. |
| Fluxo 1 · E3 | Sua categoria de chalé pode esgotar antes da virada | Vagas limitadas por categoria, inclusive a que você escolheu. |
| Fluxo 2 · E1 | Comece 2027 na Pousada Jardim 🌿 (alternativo p/ hóspedes recorrentes: "Que tal voltar pra Pousada Jardim na virada do ano?") | Pacotes de 3, 4 ou 5 diárias, com café da manhã incluso. |
| Fluxo 2 · E2 | Ainda dá tempo de planejar seu Réveillon em Monte Verde | Café da manhã completo, estrutura de lazer e a Serra pra fechar o ano. |
| Fluxo 2 · E3 | Categorias com disponibilidade limitada para o Réveillon | 10% de economia em 4 diárias, 15% em 5 diárias, por tempo limitado. |

O e-mail alternativo de Fluxo 2 · E1 usa o mesmo HTML, só muda o campo de assunto na hora de configurar o disparo pra lista de hóspedes recorrentes.

## Configuração dos fluxos (do próprio briefing, resumido aqui pra não precisar reabrir o PDF)

**Fluxo 1 (Cadastro na LP):** gatilho = conversão no formulário da LP de Réveillon → E1 imediato (buffer 15 min) → espera 2 dias → E2 → espera 3 dias → E3. Sequência linear, sem condição de abertura/clique (plano Basic).

**Fluxo 2 (Base Engajada):** disparo agendado pra uma lista montada manualmente (leads ativos + hóspedes anteriores, excluindo quem já preencheu a LP) → E1 → espera 3 dias → E2 → espera 4 dias → E3.

## Links usados (já conferidos)

- **WhatsApp**: reaproveitei os links `wa.me` já prontos do briefing, com a mensagem pré-preenchida específica de cada e-mail. Conferi a formatação de todos: número +55 35 99829-0901 (o mesmo já usado e funcionando na página de obrigado), texto pré-preenchido decodificando certinho em cada um.
- **Landing page**: usei o link real já publicado (`https://promo.jardimmonteverde.com.br/ano-novo`), com parâmetro UTM diferente em cada CTA (`utm_content=fluxo2-e1`, `fluxo2-e2`, `fluxo2-e3`) — assim dá pra cruzar no Google Analytics quantas reservas vieram de cada e-mail, como o próprio briefing sugere. Testei o link e a LP está no ar normalmente.

## Pontos que ajustei ou preciso que você confirme

1. **Números de avaliação (Fluxo 1 · E2):** o briefing trouxe 9,6 no Booking (573 avaliações), 4,9 no TripAdvisor e 4,8 no Google, os mesmos números que eu já tinha sinalizado como suspeitos lá na LP (batem exatamente com os números do Monakó, outra pousada, e provavelmente foram copiados sem querer). Pra manter consistência com o que já está no ar, usei o número que já está publicado na LP: ★ 4,5 no TripAdvisor (78 avaliações). Se vocês já tiverem os números reais e atualizados, me avisa que eu ajusto os dois lugares (LP e e-mail) de uma vez.
2. **Depoimento da hóspede:** mantive a citação exatamente como veio no briefing ("Hospedagem maravilhosa!... tudo organizado."). Como os números de avaliação vieram trocados, vale confirmar rapidinho se esse depoimento específico é mesmo de um hóspede da Jardim.
3. **Fontes:** o briefing pede "NeutralFace" (títulos) e "Raleway" (corpo), cada uma com um fallback (Georgia serifada / sans-serif limpa). E-mail não tem garantia de carregar fonte customizada, a maioria dos clientes de e-mail ignora fonte web, então usei os próprios fallbacks indicados: Georgia nos textos vivos que fariam as vezes de título, Arial/Helvetica no corpo. Os títulos que aparecem sobre a foto do banner usam a fonte Bethia de verdade (a mesma da LP e dos anúncios), porque estão desenhados direto na imagem, então não dependem do e-mail renderizar fonte nenhuma.
4. **Horário/buffer de disparo do E1 do Fluxo 1:** o briefing pede pra validar isso na configuração real do RD. Isso não dá pra confirmar por aqui, precisa checar direto na ferramenta.
5. **Cupom combinado com oferta de recorrentes:** não vi menção a isso no briefing de e-mails da Jardim (isso apareceu em outro projeto), então não se aplica aqui.

## Sobre as fotos usadas

Reaproveitei fotos já tratadas e aprovadas da campanha (as mesmas da LP e dos anúncios patrocinados), pra manter consistência visual e não depender de fotos novas do briefing que não existem na pasta:

- Fluxo 1 · E1: chalé com lareira acesa (clima aconchegante)
- Fluxo 1 · E2: casal tomando café da manhã na varanda
- Fluxo 1 · E3: quarto com toalhas sobre a cama (categoria de destaque)
- Fluxo 2 · E1: vista aérea dos chalés e da piscina ao entardecer
- Fluxo 2 · E2: fachada de um dos chalés
- Fluxo 2 · E3: quarto com varanda aberta para a mata

Se quiser trocar alguma, é só pedir.
