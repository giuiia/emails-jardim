# E-mails Outubro 2026, Pousada Jardim Monte Verde

4 e-mails (Fluxo 5, campanhas sazonais), a partir do `Briefing_Criativos_e_Emails_Outubro_Pousada_Jardim_Monte_Verde`, no mesmo modelo dos e-mails de Réveillon.

## Arquivos (pasta `Outubro/outubro/`)

- `email-natal.html`, `email-verao.html`, `email-baixa-temporada.html`, `email-planejamento.html`: HTML de produção, com as imagens apontando pro GitHub. É o link desses que vai no campo "URL do Email" do RD.
- `email-*-preview.html`: prévia com imagens embutidas, só pra abrir no navegador. Não usar no RD.
- `imagens/`: 4 banners (`outubro-banner-*.jpg`, 1200x592, otimizados a partir dos seus PNGs de 1884x930) e os logos (`outubro-logo-jardim-branco.png` no cabeçalho e `outubro-logo-jardim.png` no rodapé).

## Como subir no GitHub (repositório `emails-jardim`)

Organização combinada: cada campanha tem uma pasta própria na raiz do repositório, com os HTMLs e uma subpasta `imagens/`. Esta é a pasta `outubro`. As próximas seguem o mesmo padrão, só com o nome da campanha (ex.: `natal`, `early-booking`).

```
emails-jardim/
  emails/        (Réveillon, já publicado, não mexer)
  outubro/       (esta campanha)
    email-natal.html ... email-planejamento.html
    imagens/
```

1. No repositório, clique em Add file > Upload files.
2. Arraste a pasta `outubro` inteira (a que está em `Outubro/`), sem abrir. Ela sobe já com o nome certo na raiz.
3. Confirme o commit e abra uma imagem no navegador para testar, por exemplo `https://raw.githubusercontent.com/giuiia/emails-jardim/main/outubro/imagens/outubro-banner-natal.jpg`.
4. No RD, use no campo "URL do Email" o link raw do HTML sem "preview" no nome, por exemplo `https://raw.githubusercontent.com/giuiia/emails-jardim/main/outubro/email-natal.html`.

A pasta `emails` do Réveillon não foi alterada, então os e-mails de Réveillon continuam com as imagens funcionando. As imagens de Outubro ainda NÃO estão no ar até você subir a pasta.

## Assunto e preview text (campos do RD, fora do HTML)

| E-mail | Assunto | Preview text |
|---|---|---|
| Planejamento (abertura da campanha) | Sua próxima viagem para Monte Verde já pode estar organizada | Verão, baixa temporada ou fim de ano: o momento de planejar é agora. |
| Natal | Seu Natal em Monte Verde começa a ser planejado agora | Dezembro tem data certa para esgotar, comece a organizar sua viagem. |
| Verão | Que tal fugir do calor este verão? | Monte Verde tem verão diferente, e vale planejar com antecedência. |
| Baixa temporada | Monte Verde fica ainda melhor fora da alta temporada | Mais tranquilidade, o mesmo conforto de sempre. |

O briefing diz que o de Planejamento é o e-mail de abertura, então ele deve ser o primeiro da sequência.

## Links

- **Natal (WhatsApp):** o link do briefing usava o número 55 35 3438-1350 e vinha com `utm_source=chatgpt.com` no fim. Troquei pelo número que já usamos e funciona nos e-mails de Réveillon (55 35 99829-0901), com a mesma mensagem pré-preenchida, e tirei o `utm_source=chatgpt.com`. Se o 3438-1350 for mesmo o WhatsApp da pousada, é só me avisar.
- **Verão, Baixa temporada e Planejamento (motor de reservas):** link do hbook do briefing com UTM por e-mail (`utm_campaign=outubro2026`, `utm_content=verao`, `baixa-temporada` e `planejamento`), pra cruzar as reservas no Analytics.

## Ajustes e decisões

1. **Sem travessões:** o briefing trazia três, e todos foram trocados. No preview text do Planejamento virou dois pontos, no corpo do Verão também, e no corpo da Baixa temporada virou vírgula.
2. **Barra âmbar sob o banner:** mantive o mesmo recurso do Réveillon (texto vivo, aparece mesmo com imagem bloqueada). Como a campanha não tem desconto, a barra traz o diferencial do tema, com base na copy dos anúncios (ex.: "Café da manhã completo todos os dias e chalés com hidromassagem").
3. **Logo:** os banners chegaram sem logo, então cada e-mail tem um cabeçalho verde (`#0C2C28`, 109 px de altura, logo com 100 px de largura) acima do banner com o logo branco centralizado (`outubro-logo-jardim-branco.png`). É uma imagem separada do banner, então os banners ficaram exatamente como na sua arte. O logo dourado continua no rodapé.
4. **Texto do banner do Natal:** a arte diz "NATAL DOS SONHOS", e o briefing usa "Natal nas Montanhas" nos outros materiais. Deixei a arte como está.
5. **Sem saudação com nome, sem link de cancelar inscrição, corpo centralizado, acentos como entidades HTML:** igual ao Réveillon. O RD pode inserir o descadastro sozinho no envio.
6. **Botão único, âmbar:** um por e-mail, no fim do corpo.
