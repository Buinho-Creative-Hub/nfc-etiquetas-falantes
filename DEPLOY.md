# Deploy — Etiquetas Falantes NFC

## Render (Web Service)

- **Region:** Frankfurt (fra)
- **Build Command:** `pip install -r requirements.txt`
- **Start Command:** `python -m gunicorn app:app --bind 0.0.0.0:$PORT`
- **Runtime:** Python 3.12 (runtime.txt)
- **Plan:** Free (750h/mês, app adormece após 15 min sem uso)

## Domínio personalizado

Após deploy em `nfc-etiquetas-falantes.onrender.com`:
1. Render → Settings → Custom Domain → `nfc.buinho.eu`
2. DNS Webtuga → CNAME `nfc` → `nfc-etiquetas-falantes.onrender.com`
3. SSL automático via Let's Encrypt (~5-10 min)

## Notas
- Verificar que subdomínio `nfc` está limpo de registos zombi no DNS antes do CNAME
- Web NFC API só funciona em HTTPS — domínio personalizado é obrigatório para produção
