# Validador-de-Bandeira-de-Cartao-de-Cradito
[![wakatime](https://wakatime.com/badge/user/68660678-6b86-4b78-98df-f5f41a37e1bc/project/88c74689-cf3c-4ae5-b316-5b3c06cd6e2a.svg)](https://wakatime.com/badge/user/68660678-6b86-4b78-98df-f5f41a37e1bc/project/88c74689-cf3c-4ae5-b316-5b3c06cd6e2a)

## 💼 Sobre o projeto
Criando um Validador de Bandeiras de Cartão de Crédito com o GitHub Copilot do bootcamp

## ✅ Objetivo

Validador de Bandeira de Cartão de Crédito com o GitHub Copilot.

## 💻 Tecnologias e Ferramentas

![GitHub Copilot](https://img.shields.io/static/v1?style=for-the-badge&message=GitHub+Copilot&color=000000&logo=GitHub+Copilot&logoColor=FFFFFF&label=)
[JavaScript](https://img.shields.io/static/v1?style=for-the-badge&message=JavaScript&color=222222&logo=JavaScript&logoColor=F7DF1E&label=)

import validateCreditCard from "./utils/validador-bandeira.js";

const testCards = [
    '4532123456788888',  // VISA (16 dígitos)
    '5555555555554444',  // Mastercard
    '371449635398431',   // American Express
    '6011111111111117',  // Discover
    '30569309025904',    // Diners Club
    '3530111333300000',  // JCB
    '2014123456789012',  // EnRoute
    '8699123456789014',  // Voyager
    '6062828888666688',  // Hipercard
    '5078601870000127',  // Aura
    '9062825649040404',  // Invalido
];

testCards.forEach(cardNumber => {
    const result = validateCreditCard(cardNumber);
    console.log(`Card: ${cardNumber}`);
    console.log('Result:', result);
    console.log('------------------------');
});
