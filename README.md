# react-native-netclues-validator

[![TypeScript](https://img.shields.io/badge/TypeScript-5.2.2-blue.svg?logo=typescript&style=flat)](https://www.typescriptlang.org/)
[![React Native](https://img.shields.io/badge/React%20Native-Supported-green.svg?style=flat-square)](https://reactnative.dev/)
[![Platform](https://img.shields.io/badge/Platform-iOS%20%7C%20Android-lightgrey.svg?style=flat-square)](https://www.reactnative.dev/)
[![npm version](https://img.shields.io/npm/v/@netclues/react-native-netclues-validator.svg?style=flat-square)](https://www.npmjs.com/package/@netclues/react-native-netclues-validator)
[![npm downloads](https://img.shields.io/npm/dm/@netclues/react-native-netclues-validator.svg?style=flat-square)](https://www.npmjs.com/package/@netclues/react-native-netclues-validator)
[![license](https://img.shields.io/npm/l/@netclues/react-native-netclues-validator.svg?style=flat-square)](https://www.npmjs.com/package/@netclues/react-native-netclues-validator)


The Validator package offers a comprehensive suite of validation methods for common data types, including email, phone number, strong password, credit card number, and CVV. It also includes functionality to determine credit card types based on card numbers. With predefined regular expressions and flexible customization options, this package ensures robust and accurate validation for various use cases.

## Installation

Using npm:

```sh
npm install @netclues/react-native-netclues-validator
```

or using yarn:

```sh
yarn add @netclues/react-native-netclues-validator
```


## Usage

Importing the Validator

```js
import { Validator } from 'react-native-netclues-validator';

```
Check if a value is empty

```js
const isEmpty = Validator.isEmpty(''); // true

```
Validate an email address

```js
const isValidEmail = Validator.emailValidate('example@example.com'); // true

```
Validate a phone number

```js
const isValidPhone = Validator.phoneNumberValidate('+1234567890'); // true

```
Validate a strong password

```js
const isValidPassword = Validator.strongPasswordValidate('Password123!'); // true

```
Validate a credit card number

```js
const isValidCardNumber = Validator.creditCardNumberValidate('4111 1111 1111 1111'); // true

```
Validate a CVV code

```js
const isValidCVV = Validator.cvvValidate('123', 'Visa'); // true

```
Get the type of a credit card

```js
const cardType = Validator.getcardType('4111 1111 1111 1111'); // 'Visa'

```

## License

MIT

---
