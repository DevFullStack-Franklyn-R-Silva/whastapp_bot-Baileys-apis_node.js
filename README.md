# README

## Ferramentas

-   Node.js versão 16.16.0

## Instalação do Projeto

```bash
npm install || npm install --force
```

## Execução do Projeto

```bash
npm start
```

## Porta Padrão: 8000

API de Visualização de Código QR

Acesse `http://localhost:8000/scan` para visualizar códigos QR.

## Enviando Mensagens

### Método GET

Para visualizar um código QR, acesse:

```bash
http://localhost:8000/scan-qr
```

### Método GET

Para enviar uma mensagem, acesse:

```bash
http://localhost:8000/send-message?number=8299915558&message=oi
```

### Método POST

Para enviar uma mensagem usando o método POST, faça uma solicitação para:

```bash
http://localhost:8000/send-message
```

```bash
{
  "message": "Oi, como você está?",
  "number": "8299915558"
}
```

Nota: A imagem Base64 está sendo processada internamente.

## Observações

Se a pasta "session_auth_info" existir por padrão, exclua-a (apenas na primeira vez). Essa pasta guarda informações do usuário localmente.
