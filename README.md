# ReUse!

Aplicativo mobile desenvolvido em React Native (Expo) para incentivar o reaproveitamento e a doação de itens. Projeto da disciplina de Desenvolvimento Mobile da FIAP, Fase 2.

## Funcionalidades

- Login com sessão persistente (o usuário não precisa logar de novo ao reabrir o app)
- Renovação automática do token de acesso
- Lista de itens com busca, filtro por categoria e pull-to-refresh
- Detalhe do item
- Cadastro de item com endereço preenchido automaticamente pelo CEP
- Perfil do usuário, logout e limpeza de cache
- Cache local com validade (TTL) e funcionamento offline

## Tecnologias

- React Native + Expo
- React Navigation
- AsyncStorage e Expo SecureStore
- NetInfo

## APIs utilizadas

| API | Uso |
|-----|-----|
| [DummyJSON](https://dummyjson.com) | Autenticação e itens para reuso |
| [ViaCEP](https://viacep.com.br) | Endereço a partir do CEP |

## Como executar

```bash
git clone https://github.com/RaffaelySoares/reuse-app.git
cd reuse-app
npm install
npx expo install --fix
npx expo start
```

Abra no aplicativo Expo Go e leia o QR Code.

**Login de teste:** `emilys` / `emilyspass`

## Estrutura

```
src/
  context/    estado de autenticação
  screens/    telas do app
  services/   API, sessão e cache
```

## Autora

Raffaely Soares Pinto - RM 568568
