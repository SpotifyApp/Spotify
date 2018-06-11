Data | Responsável | Versão|
--------- | ------| --------|
11/06/2018 | José Aquiles |   1.0   |


# ✅ [UC17] - Informações de reprodução

## 1. Nome do Caso de Uso
- informações de reprodução

## 2.  Breve descrição
- Trazer informações sobre reprodução de músicas em andamento em outro dispositivo

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- aplicativo Instalado.
- Estar logado no Spotify.
- Ter acesso à internet.
- Spotify reproduzindo música em outro dispositivo. 

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. usuário inicia o aplicativo.
2. aplicativo alerta sobre reprodução ativa em outro dispositivo. [FA01]
3. usuário clica em música.
4. usuário acompanha reprodução ativa. 

## 5.2 Fluxos alternativos

FA01 - O usuário interrompe reprodução ativa em outro dispositivo
1. O usuário cancela a operação corrente.
2. O sistema redireciona o usuário para outra tela.


## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a Internet durante o procedimento
1. O sistema informa "O spotify está offline"[M1].
2. A operação é interrompida.
3. O caso de uso se encerra.

## 6 Mensagens
- [M1] O spotify está offline.