Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio |   1.0   |


# ✅ [UC12] - Criar playlist

## 1. Nome do Caso de Uso
- Criar playlist

## 2.  Breve descrição
- Cria uma nova playlist que pode ser usada para adicionar músicas que o usuário desejar.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso começa quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar biblioteca.
4. O sistema exibe as opções de funcionalidades disponíveis na biblioteca.
5. O usuário seleciona a opção Nova playlist.[FA01]
6. O sistema apresenta uma tela solicitando o nome da playlist, Imagem e descrição.
7. O usuário insere as informações requeridas e seleciona a opção criar.[FA01]
8. O sistema gera uma nova playlist.

## 5.2 Fluxos alternativos

FA01 - O usuário cancela a operação
1. O usuário cancela a operação corrente.
2. O sistema redireciona o usuário para outra tela.


## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a Internet durante o procedimento
1. O sistema informa "O spotify está offline"[M1].
2. A operação é interrompida.
3. O caso de uso se encerra.

FE02 - Aplicativo parar de funcionar
1. O sistema informa: "O aplicativo encerrou inesperadamente."[M2]
2. A operação é interrompida.
3. O caso de uso se encerra.

## 6 Mensagens
- [M1] O spotify está offline.
- [M2] O aplicativo encerrou inesperadamente.

## Regras de negócio

RN01
Descrição: Nome da playlist
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: FB06

RN02
Descrição: Descrição
Obrigatoriedade: Não
Passo​ ​do​ ​Fluxo: FB06

RN03
Descrição: Imagem
Obrigatoriedade: Não
Passo​ ​do​ ​Fluxo: FB06