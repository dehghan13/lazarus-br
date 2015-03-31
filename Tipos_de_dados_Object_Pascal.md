**Tipo de dados Integer**

Os tipos de dados integer são usados para representar números inteiros. Existem vários tipos diferentes de dados integer. Vejamos:

| Tipo | Intervalo de valores | Bytes | Com sinal |
|:-----|:---------------------|:------|:----------|
| Byte | 0 a 255 | 1 | Não |
| Word | 0 a 65535 | 2 | Não |
| ShortInt | -128 a 127 | 1 | Sim |
| SmallInt | -32768 a 32767 | 2 | Sim |
| Integer | -2147483648 a 2147483647 | 4 | Sim |
| Cardinal | 0 a 2147483648 | 4 | Não |
| LongInt | -2147483648 a 2147483647 | 4 | Sim |

 **Tipos de dados Real**



Os tipos de dados real são projetados para conter um número com uma parte fracionária. Vejamos uma tabela com tipos de dados real:

| Tipo | Intervalo | Bytes |
|:-----|:----------|:------|
| Real | ±2.9\*10<sup>39 </sup>a 1.7\*10<sup>38</sup> | 6 |
| Single | ±1.5\*10-<sup>45 </sup>a 3.4\*10<sup>38</sup> | 4 |
| Double | ±5.0\*10<sup>-324 </sup>a 1.7\*10<sup>308</sup> | 8 |
| Extended | ±3.4\*10<sup>-4932 </sup>a 1.1\*10<sup>4392</sup> | 10 |
| Comp | -2<sup>63</sup> a 2<sup>63</sup> -1 | 8 |

OBS: O tipo Comp é, na verdade, um grande inteiro, e não um real. A razão de estar incluído nesta tabela é que ele é implementado da mesma maneira dos tipos ponto flutuante. Na verdade, trata-se de um inteiro de 64 bits.

**Tipo de Dados Currency**



Na maioria das linguagens, você tem q usar um tipo de dado real para representar um valor monetário. O delphi fornece o tipo Currency especialmente para este uso. Trata-se de um tipo ponto flutuante que é compatível em relação à atribuição com todos os outros tipos de ponto flutuante. O tipo Currency tem uma precisão de 4 casas decimais, e é armazenado como um inteiro de 64 bits (onde os 4 dígitos menos significativos representam os 4 números à direita do ponto decimal).

Você pode estar se perguntando por que deveria usar o tipo currency em vez do tipo de dado real. Tipo Currency oferece duas vantagens importantes:

·  O tipo Currency tem uma precisão maior para conter números grandes;

· O tipo Currency é usado em CurrencyField e em outros componentes. Ele é compatível com tipos de banco de dados q representam dinheiro;

**Tipo de Dados Boolean**

O tipo de dados Boolean é um dos mais simples e mais usados. As variáveis desse tipo representam uma quantidade lógica; por exemplo, TRUE e FALSE.

As variáveis do tipo boolean aceitam operadores condicionais, que serão discutidos posteriormente.

**Tipos de Dados Character**

O tipo de dados caracter é bastante conhecido daqueles que já programaram em C. Esse tipo de dado foi projetado para armazenar um caracter. Um caracter tem um byte de comprimento, o que daria 256 caracteres que poderiam ser colocados em uma variável do tipo char.

O Delphi permite também o uso de caracteres do sistema UNICODE (**Unicode** é um padrão que permite aos computadores representar e manipular, de forma consistente, texto de qualquer sistema de escrita existente) utilizando de 2 Bytes.

| Tipo de Caracter | Bytes | Conteúdo |
|:-----------------|:------|:----------|
| ANSIChar ou Char | 1 | Caracter ANSI |
| WIDEChar | 2 | Caracter UNICOD |

**Tipos de dados String**

O tipo de dados String tende a ser um pouco mais útil do que o tipo Char. No Delphi, o tipo de dados String era uma concatenação de até 255 caracteres individuais. Outro termo para isso é array de caracteres. A Tabela a seguir lista os 4 tipos de Strings disponíveis no Delphi.

| Tipo String | Comprimento | Conteúdo | Terminado em Nulo |
|:------------|:------------|:----------|:------------------|
| ShortString | 255 | ANSIChar | Não |
| AnsiString | Até ~3GB | ANSIChar | Sim |
| String | 255 ou até ~3GB | ANSIChar | Sim ou Não |
| WideString | Até ~1.5GB | WideChar | Sim |

Strings maiores de 255 caracteres são alocadas dinamicamente.

**Fonte**:
http://delphiproject.blogspot.com

**Conversor de HTML to GoogleCode Wiki**:
http://toolserver.org/~diberri/cgi-bin/html2wiki