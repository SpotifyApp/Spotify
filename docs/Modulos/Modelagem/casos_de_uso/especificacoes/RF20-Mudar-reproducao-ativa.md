Data | Responsável | Versão|
--------- | ------| --------|
11/06/2018 | José Aquiles |   1.0   |


# ✅ [UC17] - Mudar Reprodução ativa

## 1. Nome do Caso de Uso
- Mudar reprodução ativa

## 2.  Breve descrição
- Mudar o dispositivo com reprodução ativa. 

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- aplicativo Instalado.
- Estar logado no Spotify.
- Ter acesso à internet.
- Spotify reproduzindo música em outro dispositivo. 

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. usuário inicia o aplicativo
2. usuário acessa informações de reprodução.
3. usuário acessa dispositivos disponíveis
4. usuário seleciona dispositivo em uso [FA01].
5. usuário ouve música no dispositivo em uso. 

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