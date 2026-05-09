# Etiquetas Falantes — NFC Talking Labels

Sistema de etiquetas de voz com NFC para pessoas com deficiência visual.  
Voice label system using NFC for visually impaired users.

## Português

Aplicação web progressiva (PWA) que permite gravar mensagens de voz e associá-las a etiquetas NFC físicas. Ao aproximar o telemóvel Android de uma etiqueta, a mensagem gravada é reproduzida automaticamente.

### Funcionalidades
- Gravação de voz por microfone
- Leitura e escrita de tags NFC (Android + Chrome)
- Armazenamento local (IndexedDB, offline-first)
- Interface totalmente acessível (ARIA, TalkBack)
- Identidade visual Buinho Educativo

### Hardware necessário
- Tags NFC NTAG213 (stickers, ~0.20€/unid)
- Telemóvel Android com Chrome

## English

Progressive web application (PWA) for recording voice messages and associating them with physical NFC labels. When an Android phone approaches a label, the recorded message plays automatically.

### Features
- Voice recording via microphone
- NFC tag read/write (Android + Chrome)
- Local storage (IndexedDB, offline-first)
- Fully accessible interface (ARIA, TalkBack compatible)
- Buinho Educativo visual identity

### Required hardware
- NTAG213 NFC sticker labels (~€0.20/unit)
- Android phone with Chrome browser

## Technical notes
- Stack: Python/Flask + Web NFC API + MediaRecorder API + IndexedDB
- Deploy: Render.com (Frankfurt region)
- iOS not supported (Apple restricts Web NFC in browser)

## License
CC-BY-SA 4.0 — [Buinho FabLab](https://buinho.pt) · Messejana, Alentejo, Portugal
