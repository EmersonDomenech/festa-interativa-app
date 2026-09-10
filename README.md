# Festa Interativa 🎉📸

Web app criado para transformar a festa de aniversário da minha esposa em uma experiência interativa para os convidados, com missões por QR Code, quiz ao vivo estilo Kahoot, ranking em tempo real e telão de fotos.

## 🧱 Arquitetura

- **Frontend:** HTML/CSS/JS puro, aplicação estática
- **Backend:** Firebase (Firestore para dados em tempo real, Storage para fotos)
- **Hospedagem:** site estático (Netlify)

## 🎯 Funcionalidades

### Missões da festa
- Convidado escaneia um QR Code, recebe uma missão sorteada
- Tira uma foto com câmera embutida no navegador (com moldura temática sobreposta ao vivo antes da captura)
- Foto é salva automaticamente no banco de fotos e gera pontos no ranking

### Quiz ao vivo (estilo Kahoot)
- Perguntas cadastradas pelo organizador direto no painel admin, sem precisar editar código
- Sincronizado entre todos os convidados: todo mundo responde a mesma pergunta ao mesmo tempo
- Cronômetro de resposta visível e configurável por pergunta
- Alternativas exibidas como símbolos coloridos (sem letras/números), com suporte a foto na pergunta
- Fluxo controlado pelo organizador: pergunta → revelar resposta → próxima pergunta
- Ranking próprio, separado do ranking de missões

### Painel administrativo
- Ativação/desativação das missões em tempo real (ex: liberar só a partir de um horário)
- Gerenciamento de participantes (editar pontos, excluir) em ambos os rankings
- Download em zip de todas as fotos tiradas
- Gerador de QR Code integrado

### Telão da festa (slideshow)
- Página dedicada para exibir em TV/notebook durante o evento
- Fotos passando aleatoriamente em destaque + fita de miniaturas rolando em tempo real
- Ranking de missões fixo ao lado, atualizando ao vivo

## 🛠️ Tecnologias

`JavaScript` `HTML/CSS` `Firebase Firestore` `Firebase Storage` `getUserMedia (câmera)` `Realtime sync`

## 📸 Contexto

Projeto pessoal criado para uma festa de aniversário, com foco em criar uma experiência divertida e sincronizada para os convidados sem depender de apps de terceiros.
