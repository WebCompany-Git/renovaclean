# RENOVA CLEAN — Guia de SEO e Google (negócio por agendamento)

A RENOVA CLEAN não tem local fixo e atende no local do cliente. Para o Google isto é um **negócio de área de serviço** (*service-area business*). Todo o SEO deste projecto foi preparado para isso: **sem morada pública**, com zonas de atendimento (Luanda, Zango, Icolo e Bengo).

---

## 1. Ficheiros SEO incluídos

| Ficheiro | Para quê |
|---|---|
| `index.html` (`<head>`) | Título, descrição, canonical, hreflang, Open Graph (WhatsApp/Facebook), Twitter, ícones e **dados estruturados JSON-LD** (negócio local, serviços, preços, FAQ, zonas, redes sociais) |
| `robots.txt` | Autoriza os motores de busca e indica o sitemap |
| `sitemap.xml` | Lista a página e as imagens antes/depois para o Google |
| `site.webmanifest` | Nome, cor e ícones do site em telemóveis |
| `404.html` | Página de erro com `noindex` (evita páginas inexistentes no Google) |
| `assets/og-image.jpg` | Imagem 1200×630 que aparece quando o link é partilhado no WhatsApp/Facebook |
| `assets/icons/*` | Favicon `.ico`, PNG 48/96/192/512 e `apple-touch-icon` (o Google exige favicon em múltiplos de 48 px) |
| `assets/logo.webp` / `logo.png` | Logótipo leve (29 KB em WebP) que substituiu o SVG de 242 KB usado no menu e rodapé |

---

## 2. Antes de publicar

1. **Domínio:** já configurado como `https://renova-clean.vercel.app` (sem `www`) em `index.html`, `robots.txt` e `sitemap.xml`. Se mais tarde comprar um domínio próprio (ex.: `renovaclean.ao`), substitua este endereço nesses 3 ficheiros e adicione o domínio na Vercel (Settings → Domains).
2. **Vercel:** o HTTPS já vem activo. Se mais tarde ligar um domínio próprio, deixe a Vercel redireccionar a versão `www` para a principal. O `404.html` é usado automaticamente pela Vercel.
3. **Atenção:** um endereço `.vercel.app` funciona no Google, mas um domínio próprio dá mais confiança e deixa de depender da Vercel — recomendado quando o negócio crescer.
4. Actualizar `<lastmod>` no `sitemap.xml` sempre que mudar o conteúdo.
5. Confirmar os dados que estão no JSON-LD: telefone, preços, horário (24/24h), zonas. Se o horário não for mesmo 24/24h, altere em `openingHoursSpecification` e no rodapé — **o Google compara o site com o Perfil de Empresa**.

---

## 3. Google Search Console (fazer no dia da publicação)

1. Aceder a <https://search.google.com/search-console> e adicionar o site (propriedade "Prefixo do URL" é a mais simples).
2. Verificar a propriedade: escolha "Etiqueta HTML", copie o código e descomente a linha `google-site-verification` no `<head>` do `index.html`.
3. Em **Sitemaps**, submeter `sitemap.xml`.
4. Em **Inspeção de URL**, colar a página inicial → *Pedir indexação*.
5. Repetir em <https://www.bing.com/webmasters> (Bing também alimenta outros motores).

---

## 4. Perfil de Empresa no Google (Google Business Profile)

É o que faz a empresa aparecer em "limpeza de sofás perto de mim" e no Google Maps.

### Criar como negócio de área de serviço
- Pergunta "Adicionar localização que os clientes possam visitar?" → **Não**. 
- **Não coloque morada** (nem a de casa). Em "Áreas de serviço" adicione: `Luanda`, `Zango` (Viana), `Icolo e Bengo` — e mais bairros/municípios que realmente atende (até 20).
- **Nome:** exactamente `RENOVA CLEAN` (sem acrescentar palavras-chave como "Limpeza de sofás Luanda" — o Google suspende por isso).
- **Categoria principal:** a que melhor descreve o serviço (procure "estofos" / *Upholstery cleaning service*). **Secundárias:** *Carpet cleaning service*, *Mattress cleaning service* (se existir na lista em português), *Car detailing service* / limpeza de interior de viaturas, *Cleaning service*. A lista exacta de categorias muda — escolha as mais próximas no painel.
- **Telefone:** `+244 936 853 785` — o mesmo do site. **Website:** o domínio real.
- **Horário:** use o horário real. Só marque "24 horas" se atende mesmo a qualquer hora; caso contrário defina o horário de atendimento por marcação.
- **Redes sociais:** adicione Instagram, Facebook, TikTok.

### Descrição (máx. 750 caracteres — pronta a colar)
> A RENOVA CLEAN faz higienização profissional de sofás, colchões, cadeiras, poltronas, tapetes e interiores de viaturas, directamente em sua casa ou empresa, em Luanda, Zango e Icolo e Bengo. Atendemos por agendamento: envie uma foto do item pelo WhatsApp, receba o orçamento e marque o melhor dia e hora. Usamos extração profissional para remover sujidade e reduzir a humidade, com cuidado pelo material de cada peça. Atendemos também escritórios, restaurantes, hotéis, salões e clínicas. Não troque. Renove.

### Serviços e preços (crie em "Serviços", com os mesmos valores do site)
- Higienização de sofá — a partir de 9.900 Kz (até 3 lugares)
- Pacote Casa Renovada — 25.000 Kz (sofá + colchão de casal + 2 cadeiras)
- Higienização de interior de viatura — a partir de 15.000 Kz
- Colchões · Cadeiras e poltronas · Tapetes · Higienização empresarial — "sob orçamento"

### Fotografias (o que mais pesa na confiança)
Carregue **fotos reais**: antes/depois de trabalhos, equipa a trabalhar, equipamento, logótipo, capa. Mínimo 10 no início, depois 2–4 por semana. Evite fotos de bancos de imagem.

### Verificação
Como não há morada, o Google normalmente pede **vídeo de verificação** (mostrar equipamento, produtos, veículo/uniforme com logótipo e a actividade). As opções disponíveis variam por país — siga o que o painel oferecer.

### Depois de verificado
- **Avaliações:** peça a cada cliente satisfeito. Use o link curto de avaliação (painel → "Pedir avaliações") e envie por WhatsApp logo após o serviço. Nunca compre nem invente avaliações — o Google remove e pode suspender o perfil.
- Responda a todas as avaliações.
- **Publicações** (Updates): 1 por semana com um antes/depois.
- Active as **mensagens/chat** e o botão de ligar.

---

## 5. Consistência (NAP) — regra de ouro

Nome **RENOVA CLEAN**, telefone **+244 936 853 785** e zonas devem ser **idênticos** no site, Google, Facebook, Instagram, TikTok e WhatsApp Business. Verifique também o identificador do Instagram: o site aponta para `@renovamclean` (com "m") e o TikTok é `@renovaclean45` — confirme se o do Instagram está mesmo correcto.

---

## 6. O que fazer a seguir para subir no Google

O site é de **uma só página**, o que limita o posicionamento. Por ordem de impacto:

1. **Páginas por serviço e por zona** (ex.: `/higienizacao-de-sofas-luanda`, `/limpeza-de-colchoes-zango`, `/limpeza-interior-de-carros-luanda`), cada uma com 300+ palavras originais, fotos reais e botão de WhatsApp. Cada página nova entra no `sitemap.xml`.
2. **Mencionar as zonas no texto** da página (hoje Zango e Icolo e Bengo só aparecem no rodapé). Uma secção "Zonas de atendimento" ajuda.
3. **Avaliações reais** no Google; quando tiver várias, pode adicionar `aggregateRating` ao JSON-LD — **só com avaliações verdadeiras**.
4. **Blog/guias curtos** ("Como tirar nódoas de sofá de tecido", "Quanto tempo demora a secar um sofá"…).
5. **Desempenho:** a imagem principal vem do Unsplash (link externo) — descarregue-a, converta para WebP (≤150 KB) e guarde em `img/`; converta `antes.jpg`/`depois.jpg` para WebP. Há 3 folhas de estilo externas (Google Fonts, Font Awesome, Lucide) que atrasam a primeira pintura — mais tarde convém reduzir.
6. **Backlinks locais:** perfis no Facebook, Instagram, TikTok com o link do site, directórios angolanos de empresas, parcerias com condomínios, imobiliárias e restaurantes.

---

## 7. Notas honestas

- SEO demora: normalmente **semanas a meses** para ver resultados; o Perfil de Empresa costuma mostrar efeito mais cedo.
- O marcado **FAQ** continua válido, mas o Google já só mostra caixas de perguntas expandidas em poucos tipos de sites; mantém-se porque ajuda a máquina a perceber o conteúdo.
- O JSON-LD não inclui avaliações nem morada de rua de propósito.
- Para testar: <https://search.google.com/test/rich-results> (colar o URL) e <https://validator.schema.org>.
