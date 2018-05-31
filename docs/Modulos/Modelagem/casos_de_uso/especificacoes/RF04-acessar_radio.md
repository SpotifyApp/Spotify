Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Geovanne Santos |   1.0   |


# ✅ [UC03] - Acessar rádio

## 1. Nome do Caso de Uso
- Acessar rádio

## 2.  Breve descrição
- O usuário deseja que o spotify escolha as músicas que serão tocadas, ou que possa criar qualquer estação de rádio escolhendo os artistas e playlists que irão basear a rádio.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta premium.
- Ter o aplicativo do Spotify instalado
- Ter feito o login.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso começa quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar rádio.
4. O sistema exibe as opções de funcionalidades disponíveis na página rádio.[FA01] [FA02]
5. O usuário seleciona uma rádio baseada nas recomendações que spotify fez(de acordo com as músicas que o usuário ouve)
6. O sistema começa a tocar a rádio selecionada.

## 5.2 Fluxos alternativos

FA01 - O usuário ouve uma rádio de acordo com o gênero dela
1. O usuário seleciona uma rádio de acordo com o gênero dela(rock, samba, mpb, entre outros) FE01
2. O sistema começa a tocar a rádio selecionada.


FA02 - O usuário deseja criar uma estação de rádio, baseada em algumas playlists e artistas
1. O usuário seleciona a opção de criar uma rádio.
2. O sistema direciona o usuário para a página de criar rádio. FE01
3. O usuário escolhe os artistas e playlists que a rádio deve se basear, pelo campo de busca.
4. O sistema gera a rádio.
5. O usuário poderá somente ouvir a rádio ou adiciona-lá a biblioteca.

## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a Internet durante o procedimento
1. O sistema informa "O spotify está offline"[M1].
2. A operação é interrompida.
3. O caso de uso se encerra.

FE02 - Aplicativo parar de funcionar
1. O sistema informa: "O aplicativo encerrou inesperadamente."[M2]
2. A operação é interrompida.
3. O caso de uso se encerra.

FE03 - O nome que o usuário procura não existe
1. O sistema informa [M1].

## 6 Mensagens
- [M1] O spotify está offline.
- [M2] O aplicativo encerrou inesperadamente.
- [M3] O nome desejado não existe, por favor tente um nome diferente.
