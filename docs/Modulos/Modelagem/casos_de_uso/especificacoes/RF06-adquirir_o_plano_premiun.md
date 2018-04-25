Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

# ✅ [UC06] - Adquirir o plano premiun

## 1. Nome do Caso de Uso
- Adquirir o plano premiun

## 2.  Breve descrição
- Comprar o plano premiun, com mais funcionalidades.

## 3.  Atores
- Usuário free.

## 4.  Pré-Condição
- O usuário deve ser free.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário clica em adquirir plano premiun.
- Usuário coloca as informações para o contrato do plano ser firmado.
- O usuário escolhe a forma de pagamento.
- O usuário paga a fatura e mude do plano free para o plano premiun de imediato.

## 5.2 Fluxos alternativos

- [FA01]
- Adquirir um plano premiun, pelo pacote estudantil.

- [FA02]
- Adquirir um plano premiun, pelo pacote família.

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário coloca alguma informação errada:
- O sistema identifica a resposta inválida .
- O sistema permanece na mesma página.
- O sistema destaca o box com a informação inválida.

- [FE03] Usuário não paga a fatura:
- O sistema não muda de free para premiun .


## 6 Mensagens
- [M1] O dado da mensagem está inválido, por favor insira novamente o dado da mensagem.
