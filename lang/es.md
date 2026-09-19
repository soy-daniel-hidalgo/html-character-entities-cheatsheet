<div>
  <a href="http://www.w3.org/html/logo/">
    <img src="https://www.w3.org/html/logo/badge/html5-badge-h-semantics.png" width="133" height="64" align="left" alt="HTML5 impulsado por la semántica" title="HTML5 impulsado por la semántica">
  </a>
  <br>

  <h1 align="right">Cheat sheet sobre entidades de caracteres en HTML</h1>
</div>

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../assets/es/banner-dark-mode-es.png" alt="Banner del repositorio en tema oscuro" />
    <source media="(prefers-color-scheme: light)" srcset="../assets/es/banner-light-mode-es.png" alt="Banner del repositorio en tema claro" />
    <img src="../assets/es/banner-light-mode-es.png" alt="Tema predeterminado del banner del repositorio" />
  </picture>
</div>

## 📑 Acerca de

Las **entidades de caracteres** te permiten mostrar caracteres especiales y símbolos dentro de documentos **HTML** que no están disponibles en la codificación ordinaria de caracteres (**charset**). Estos caracteres especiales se deben reemplazar por **entidades de caracteres** para evitar que el navegador los interprete como código HTML o los renderice de forma incorrecta.

Este sencillo *cheat sheet* ofrece una referencia rápida para ayudarte a navegar por este mar de caracteres, glifos y símbolos. Cubriremos su uso, tipos y buenas prácticas para crear contenido accesible y semánticamente correcto.

🫶 **¡Las contribuciones son bienvenidas!** Siéntete libre de:

- Corregir errores gramaticales y mejorar la legibilidad.
- Añadir nuevos caracteres, glifos y símbolos.
- Traducir este proyecto a tu idioma.
- Mejorar las explicaciones y proponer otras ideas.

---

## 📋 Tabla de contenidos

- [📑 Acerca de](#-acerca-de)
- [📎 Tipos de entidades de caracteres](#-tipos-de-entidades-de-caracteres)
- [📓 Buenas prácticas y recomendaciones](#buenas-prácticas-y-recomendaciones)
- [📜 Lista de entidades de caracteres en HTML](#-lista-de-entidades-de-caracteres-en-html)
- [🌎 Traducciones](#-traducciones)
- [🤝 Contribuir](#-contribuir)
- [📄 Licencias y derechos de autor](#-licencias-y-derechos-de-autor)

---

## 📎 Tipos de entidades de caracteres

Las entidades de caracteres en HTML son códigos que se utilizan para mostrar caracteres reservados o símbolos especiales, como letras con acentos, signos diacríticos, emojis y caracteres que no se encuentran en un teclado estándar, sin interferir con el procesamiento o *parsing*) de HTML.

Existen tres formas de representarlas:

1. **Por nombre de la entidad:** Varias entidades están representadas por un nombre estandarizado, único y legible para los seres humanos, como `&copy;` para el símbolo de derechos de autor (&copy;) y `&gt;` para el signo mayor que (&gt;), que es una abreviatura del inglés: *greater than*.
2. **Códigos decimales:** Representados por el valor decimal en Unicode del carácter, precedido por `&#`, por ejemplo `&#169;` representa el símbolo de derechos de autor (&#169;) y `&#120506;` representa el carácter matemático sigma (&#120506;).
3. **Códigos hexadecimales:** Representados por el valor hexadecimal en Unicode del carácter, precedido por `&#x`, por ejemplo `&#x00A9;` representa el símbolo de derechos de autor (&#x00A9;) y `&#x03A9;` para la letra griega omega (&#x03A9;).

> [!TIP]
> Tanto el formato decimal como el hexadecimal son conocidos como **Entidades numéricas**.

---

## 📓 Buenas prácticas y recomendaciones

- **Optar por entidades con nombre cuando sea posible:** Utiliza entidades con nombre para los caracteres comunes con el fin de mejorar la legibilidad del código. Las entidades por nombre son más fáciles de recordar que las numéricas, lo que las hace más sencillas de leer y mantener.

> [!NOTE]
> Los nombres de las entidades distinguen entre mayúsculas y minúsculas (*case-sensitive*). Escribe siempre los nombres de las entidades en minúsculas.

- **Utilizar entidades numéricas para caracteres menos comunes:** Muchos caracteres como `U+2691` (⚑) no tienen un equivalente por nombre. En estos casos, utiliza códigos decimales o hexadecimales en su lugar.

- **Priorizar la accesibilidad:** Asegúrate de que las entidades de caracteres sigan siendo accesibles para los lectores de pantalla y otras tecnologías de asistencia proporcionando texto alternativo o contexto cuando sea necesario.

> [!TIP]
> Especifica siempre la codificación de caracteres como UTF-8 (`<meta charset="UTF-8">`) al principio de cada documento HTML. UTF-8 admite de forma nativa casi todos los caracteres, lo que garantiza que los navegadores muestren el contenido correctamente y elimina la necesidad de usar entidades de caracteres en la mayoría de los casos.

> [!WARNING]
> Los navegadores web solo pueden representar un carácter si el dispositivo del usuario tiene instalada una fuente que lo admita. Si un carácter no está disponible en las fuentes instaladas, por lo general se mostrará como un cuadro u otro símbolo como *placeholder*.

---

## 📜 Lista de entidades de caracteres en HTML

| Carácter | Descripción | Entidad por nombre | Código decimal | Código hexadecimal |
| :---: | --- | :---: | :---: | :---: |
| " | Comilla doble | `&quot;` | `&#34;` | `&#x0022;` |
| `&` | Ampersand (*Et*) | `&amp;` | `&#38;` | `&#x0026;` |
| `'` | Apóstrofo | `&apos;` | `&#39;` | `&#x0027;` |
| `<` | Signo menor que | `&lt;` | `&#60;` | `&#x003C;` |
| `>` | Signo mayor que | `&gt;` | `&#62;` | `&#x003E;` |
| ` ` | Espacio de no separación | `&nbsp;` | `&#160;` | `&#x00A0;` |
| `¡` | Signo de exclamación de apertura | `&iexcl;` | `&#161;` | `&#x00A1;` |
| `¢` | Símbolo de centavo | `&cent;` | `&#162;` | `&#x00A2;` |
| `£` | Símbolo de libra | `&pound;` | `&#163;` | `&#x00A3;` |
| `¤` | Símbolo de moneda | `&curren;` | `&#164;` | `&#x00A4;` |
| `¥` | Símbolo de yen | `&yen;` | `&#165;` | `&#x00A5;` |
| `¦` | Barra rota | `&brvbar;` | `&#166;` | `&#x00A6;` |
| `§` | Signo de sección | `&sect;` | `&#167;` | `&#x00A7;` |
| `¨` | Diéresis | `&uml;` | `&#168;` | `&#x00A8;` |
| `©` | Símbolo de derechos de autor | `&copy;` | `&#169;` | `&#x00A9;` |
| `ª` | Indicador ordinal femenino | `&ordf;` | `&#170;` | `&#x00AA;` |
| `«` | Comillas angulares dobles de apertura | `&laquo;` | `&#171;` | `&#x00AB;` |
| `¬` | Signo de negación lógica | `&not;` | `&#172;` | `&#x00AC;` |
| `­` | Guion blando | `&shy;` | `&#173;` | `&#x00AD;` |
| `®` | Marca registrada | `&reg;` | `&#174;` | `&#x00AE;` |
| `¯` | Macrón | `&macr;` | `&#175;` | `&#x00AF;` |
| `°` | Símbolo de grado | `&deg;` | `&#176;` | `&#x00B0;` |
| `±` | Signo más-menos | `&plusmn;` | `&#177;` | `&#x00B1;` |
| `²` | Superíndice dos | `&sup2;` | `&#178;` | `&#x00B2;` |
| `³` | Superíndice tres | `&sup3;` | `&#179;` | `&#x00B3;` |
| `´` | Acento agudo | `&acute;` | `&#180;` | `&#x00B4;` |
| `µ` | Signo de micro | `&micro;` | `&#181;` | `&#x00B5;` |
| `¶` | Signo de párrafo | `&para;` | `&#182;` | `&#x00B6;` |
| `·` | Punto medio | `&middot;` | `&#183;` | `&#x00B7;` |
| `¸` | Cedilla | `&cedil;` | `&#184;` | `&#x00B8;` |
| `¹` | Superíndice uno | `&sup1;` | `&#185;` | `&#x00B9;` |
| `º` | Indicador ordinal masculino | `&ordm;` | `&#186;` | `&#x00BA;` |
| `»` | Comillas angulares dobles de cierre | `&raquo;` | `&#187;` | `&#x00BB;` |
| `¼` | Fracción de un cuarto | `&frac14;` | `&#188;` | `&#x00BC;` |
| `½` | Fracción de un medio | `&frac12;` | `&#189;` | `&#x00BD;` |
| `¾` | Fracción de tres cuartos | `&frac34;` | `&#190;` | `&#x00BE;` |
| `¿` | Signo de interrogación de apertura | `&iquest;` | `&#191;` | `&#x00BF;` |
| `À` | Letra latina A mayúscula con acento grave | `&Agrave;` | `&#192;` | `&#x00C0;` |
| `Á` | Letra latina A mayúscula con acento agudo | `&Aacute;` | `&#193;` | `&#x00C1;` |
| `Â` | Letra latina A mayúscula con acento circunflejo | `&Acirc;` | `&#194;` | `&#x00C2;` |
| `Ã` | Letra latina A mayúscula con virgulilla | `&Atilde;` | `&#195;` | `&#x00C3;` |
| `Ä` | Letra latina A mayúscula con diéresis | `&Auml;` | `&#196;` | `&#x00C4;` |
| `Å` | Letra latina A mayúscula con anillo superior | `&Aring;` | `&#197;` | `&#x00C5;` |
| `Æ` | Ligadura latina AE mayúscula | `&AElig;` | `&#198;` | `&#x00C6;` |
| `Ç` | Letra latina C mayúscula con cedilla | `&Ccedil;` | `&#199;` | `&#x00C7;` |
| `È` | Letra latina E mayúscula con acento grave | `&Egrave;` | `&#200;` | `&#x00C8;` |
| `É` | Letra latina E mayúscula con acento agudo | `&Eacute;` | `&#201;` | `&#x00C9;` |
| `Ê` | Letra latina E mayúscula con acento circunflejo | `&Ecirc;` | `&#202;` | `&#x00CA;` |
| `Ë` | Letra latina E mayúscula con diéresis | `&Euml;` | `&#203;` | `&#x00CB;` |
| `Ì` | Letra latina I mayúscula con acento grave | `&Igrave;` | `&#204;` | `&#x00CC;` |
| `Í` | Letra latina I mayúscula con acento agudo | `&Iacute;` | `&#205;` | `&#x00CD;` |
| `Î` | Letra latina I mayúscula con acento circunflejo | `&Icirc;` | `&#206;` | `&#x00CE;` |
| `Ï` | Letra latina I mayúscula con diéresis | `&Iuml;` | `&#207;` | `&#x00CF;` |
| `Ð` | Letra latina Eth mayúscula | `&ETH;` | `&#208;` | `&#x00D0;` |
| `Ñ` | Letra latina N mayúscula con virgulilla | `&Ntilde;` | `&#209;` | `&#x00D1;` |
| `Ò` | Letra latina O mayúscula con acento grave | `&Ograve;` | `&#210;` | `&#x00D2;` |
| `Ó` | Letra latina O mayúscula con acento agudo | `&Oacute;` | `&#211;` | `&#x00D3;` |
| `Ô` | Letra latina O mayúscula con acento circunflejo | `&Ocirc;` | `&#212;` | `&#x00D4;` |
| `Õ` | Letra latina O mayúscula con virgulilla | `&Otilde;` | `&#213;` | `&#x00D5;` |
| `Ö` | Letra latina O mayúscula con diéresis | `&Ouml;` | `&#214;` | `&#x00D6;` |
| `×` | Signo de multiplicación | `&times;` | `&#215;` | `&#x00D7;` |
| `Ø` | Letra latina O mayúscula con barra diagonal | `&Oslash;` | `&#216;` | `&#x00D8;` |
| `Ù` | Letra latina U mayúscula con acento grave | `&Ugrave;` | `&#217;` | `&#x00D9;` |
| `Ú` | Letra latina U mayúscula con acento agudo | `&Uacute;` | `&#218;` | `&#x00DA;` |
| `Û` | Letra latina U mayúscula con acento circunflejo | `&Ucirc;` | `&#219;` | `&#x00DB;` |
| `Ü` | Letra latina U mayúscula con diéresis | `&Uuml;` | `&#220;` | `&#x00DC;` |
| `Ý` | Letra latina Y mayúscula con acento agudo | `&Yacute;` | `&#221;` | `&#x00DD;` |
| `Þ` | Letra latina Thorn mayúscula | `&THORN;` | `&#222;` | `&#x00DE;` |
| `ß` | Letra latina s minúscula alemana (*Eszett*) | `&szlig;` | `&#223;` | `&#x00DF;` |
| `à` | Letra latina a minúscula con acento grave | `&agrave;` | `&#224;` | `&#x00E0;` |
| `á` | Letra latina a minúscula con acento agudo | `&aacute;` | `&#225;` | `&#x00E1;` |
| `â` | Letra latina a minúscula con acento circunflejo | `&acirc;` | `&#226;` | `&#x00E2;` |
| `ã` | Letra latina a minúscula con virgulilla | `&atilde;` | `&#227;` | `&#x00E3;` |
| `ä` | Letra latina a minúscula con diéresis | `&auml;` | `&#228;` | `&#x00E4;` |
| `å` | Letra latina a minúscula con anillo superior | `&aring;` | `&#229;` | `&#x00E5;` |
| `æ` | Ligadura latina ae minúscula | `&aelig;` | `&#230;` | `&#x00E6;` |
| `ç` | Letra latina c minúscula con cedilla | `&ccedil;` | `&#231;` | `&#x00E7;` |
| `è` | Letra latina e minúscula con acento grave | `&egrave;` | `&#232;` | `&#x00E8;` |
| `é` | Letra latina e minúscula con acento agudo | `&eacute;` | `&#233;` | `&#x00E9;` |
| `ê` | Letra latina e minúscula con acento circunflejo | `&ecirc;` | `&#234;` | `&#x00EA;` |
| `ë` | Letra latina e minúscula con diéresis | `&euml;` | `&#235;` | `&#x00EB;` |
| `ì` | Letra latina i minúscula con acento grave | `&igrave;` | `&#236;` | `&#x00EC;` |
| `í` | Letra latina i minúscula con acento agudo | `&iacute;` | `&#237;` | `&#x00ED;` |
| `î` | Letra latina i minúscula con acento circunflejo | `&icirc;` | `&#238;` | `&#x00EE;` |
| `ï` | Letra latina i minúscula con diéresis | `&iuml;` | `&#239;` | `&#x00EF;` |
| `ð` | Letra latina eth minúscula | `&eth;` | `&#240;` | `&#x00F0;` |
| `ñ` | Letra latina n minúscula con virgulilla | `&ntilde;` | `&#241;` | `&#x00F1;` |
| `ò` | Letra latina o minúscula con acento grave | `&ograve;` | `&#242;` | `&#x00F2;` |
| `ó` | Letra latina o minúscula con acento agudo | `&oacute;` | `&#243;` | `&#x00F3;` |
| `ô` | Letra latina o minúscula con acento circunflejo | `&ocirc;` | `&#244;` | `&#x00F4;` |
| `õ` | Letra latina o minúscula con virgulilla | `&otilde;` | `&#245;` | `&#x00F5;` |
| `ö` | Letra latina o minúscula con diéresis | `&ouml;` | `&#246;` | `&#x00F6;` |
| `÷` | Signo de división | `&divide;` | `&#247;` | `&#x00F7;` |
| `ø` | Letra latina o minúscula con barra diagonal | `&oslash;` | `&#248;` | `&#x00F8;` |
| `ù` | Letra latina u minúscula con acento grave | `&ugrave;` | `&#249;` | `&#x00F9;` |
| `ú` | Letra latina u minúscula con acento agudo | `&uacute;` | `&#250;` | `&#x00FA;` |
| `û` | Letra latina u minúscula con acento circunflejo | `&ucirc;` | `&#251;` | `&#x00FB;` |
| `ü` | Letra latina u minúscula con diéresis | `&uuml;` | `&#252;` | `&#x00FC;` |
| `ý` | Letra latina y minúscula con acento agudo | `&yacute;` | `&#253;` | `&#x00FD;` |
| `þ` | Letra latina thorn minúscula | `&thorn;` | `&#254;` | `&#x00FE;` |
| `ÿ` | Letra latina y minúscula con diéresis | `&yuml;` | `&#255;` | `&#x00FF;` |
| `Œ` | Ligadura latina OE mayúscula | `&OElig;` | `&#338;` | `&#x0152;` |
| `œ` | Ligadura latina oe minúscula | `&oelig;` | `&#339;` | `&#x0153;` |
| `Š` | Letra latina S mayúscula con carón | `&Scaron;` | `&#352;` | `&#x0160;` |
| `š` | Letra latina s minúscula con carón | `&scaron;` | `&#353;` | `&#x0161;` |
| `Ÿ` | Letra latina Y mayúscula con diéresis | `&Yuml;` | `&#376;` | `&#x0178;` |
| `ƒ` | Letra latina f minúscula con gancho | `&fnof;` | `&#402;` | `&#x0192;` |
| `ˆ` | Acento circunflejo modificador | `&circ;` | `&#710;` | `&#x02C6;` |
| `˜` | Virgulilla pequeña | `&tilde;` | `&#732;` | `&#x02DC;` |
| `Α` | Letra griega Alfa mayúscula | `&Alpha;` | `&#913;` | `&#x0391;` |
| `Β` | Letra griega Beta mayúscula | `&Beta;` | `&#914;` | `&#x0392;` |
| `Γ` | Letra griega Gamma mayúscula | `&Gamma;` | `&#915;` | `&#x0393;` |
| `Δ` | Letra griega Delta mayúscula | `&Delta;` | `&#916;` | `&#x0394;` |
| `Ε` | Letra griega Épsilon mayúscula | `&Epsilon;` | `&#917;` | `&#x0395;` |
| `Ζ` | Letra griega Zeta mayúscula | `&Zeta;` | `&#918;` | `&#x0396;` |
| `Η` | Letra griega Eta mayúscula | `&Eta;` | `&#919;` | `&#x0397;` |
| `Θ` | Letra griega Theta mayúscula | `&Theta;` | `&#920;` | `&#x0398;` |
| `Ι` | Letra griega Iota mayúscula | `&Iota;` | `&#921;` | `&#x0399;` |
| `Κ` | Letra griega Kappa mayúscula | `&Kappa;` | `&#922;` | `&#x039A;` |
| `Λ` | Letra griega Lambda mayúscula | `&Lambda;` | `&#923;` | `&#x039B;` |
| `Μ` | Letra griega Mu mayúscula | `&Mu;` | `&#924;` | `&#x039C;` |
| `Ν` | Letra griega Nu mayúscula | `&Nu;` | `&#925;` | `&#x039D;` |
| `Ξ` | Letra griega Xi mayúscula | `&Xi;` | `&#926;` | `&#x039E;` |
| `Ο` | Letra griega Ómicron mayúscula | `&Omicron;` | `&#927;` | `&#x039F;` |
| `Π` | Letra griega Pi mayúscula | `&Pi;` | `&#928;` | `&#x03A0;` |
| `Ρ` | Letra griega Rho mayúscula | `&Rho;` | `&#929;` | `&#x03A1;` |
| `Σ` | Letra griega Sigma mayúscula | `&Sigma;` | `&#931;` | `&#x03A3;` |
| `Τ` | Letra griega Tau mayúscula | `&Tau;` | `&#932;` | `&#x03A4;` |
| `Υ` | Letra griega Ípsilon mayúscula | `&Upsilon;` | `&#933;` | `&#x03A5;` |
| `Φ` | Letra griega Phi mayúscula | `&Phi;` | `&#934;` | `&#x03A6;` |
| `Χ` | Letra griega Chi mayúscula | `&Chi;` | `&#935;` | `&#x03A7;` |
| `Ψ` | Letra griega Psi mayúscula | `&Psi;` | `&#936;` | `&#x03A8;` |
| `Ω` | Letra griega Omega mayúscula | `&Omega;` | `&#937;` | `&#x03A9;` |
| `α` | Letra griega alfa minúscula | `&alpha;` | `&#945;` | `&#x03B1;` |
| `β` | Letra griega beta minúscula | `&beta;` | `&#946;` | `&#x03B2;` |
| `γ` | Letra griega gamma minúscula | `&gamma;` | `&#947;` | `&#x03B3;` |
| `δ` | Letra griega delta minúscula | `&delta;` | `&#948;` | `&#x03B4;` |
| `ε` | Letra griega épsilon minúscula | `&epsilon;` | `&#949;` | `&#x03B5;` |
| `ζ` | Letra griega zeta minúscula | `&zeta;` | `&#950;` | `&#x03B6;` |
| `η` | Letra griega eta minúscula | `&eta;` | `&#951;` | `&#x03B7;` |
| `θ` | Letra griega theta minúscula | `&theta;` | `&#952;` | `&#x03B8;` |
| `ι` | Letra griega iota minúscula | `&iota;` | `&#953;` | `&#x03B9;` |
| `κ` | Letra griega kappa minúscula | `&kappa;` | `&#954;` | `&#x03BA;` |
| `λ` | Letra griega lambda minúscula | `&lambda;` | `&#955;` | `&#x03BB;` |
| `μ` | Letra griega mu minúscula | `&mu;` | `&#956;` | `&#x03BC;` |
| `ν` | Letra griega nu minúscula | `&nu;` | `&#957;` | `&#x03BD;` |
| `ξ` | Letra griega xi minúscula | `&xi;` | `&#958;` | `&#x03BE;` |
| `ο` | Letra griega ómicron minúscula | `&omicron;` | `&#959;` | `&#x03BF;` |
| `π` | Letra griega pi minúscula | `&pi;` | `&#960;` | `&#x03C0;` |
| `ρ` | Letra griega rho minúscula | `&rho;` | `&#961;` | `&#x03C1;` |
| `ς` | Letra griega sigma final minúscula | `&sigmaf;` | `&#962;` | `&#x03C2;` |
| `σ` | Letra griega sigma minúscula | `&sigma;` | `&#963;` | `&#x03C3;` |
| `τ` | Letra griega tau minúscula | `&tau;` | `&#964;` | `&#x03C4;` |
| `υ` | Letra griega ípsilon minúscula | `&upsilon;` | `&#965;` | `&#x03C5;` |
| `φ` | Letra griega phi minúscula | `&phi;` | `&#966;` | `&#x03C6;` |
| `χ` | Letra griega chi minúscula | `&chi;` | `&#967;` | `&#x03C7;` |
| `ψ` | Letra griega psi minúscula | `&psi;` | `&#968;` | `&#x03C8;` |
| `ω` | Letra griega omega minúscula | `&omega;` | `&#969;` | `&#x03C9;` |
| `ϑ` | Símbolo griego theta | `&thetasym;` | `&#977;` | `&#x03D1;` |
| `ϒ` | Símbolo griego ípsilon con gancho | `&upsih;` | `&#978;` | `&#x03D2;` |
| `ϖ` | Símbolo griego pi | `&piv;` | `&#982;` | `&#x03D6;` |
| `–` | Semirraya | `&ndash;` | `&#8211;` | `&#x2013;` |
| `—` | Raya | `&mdash;` | `&#8212;` | `&#x2014;` |

---

## 🌎 Traducciones

Este proyecto está disponible en los siguientes idiomas:

| Idioma | Enlace |
| --- | --- |
| 🇬🇧 Inglés | [HTML Character Entities Cheat Sheet](../README.md) |
| 🇪🇸 Español | **Cheat sheet sobre entidades de caracteres en HTML** — Ud. está aquí **◝(ᵔᵕᵔ)◜** |

---

## 🤝 Contribuir

**¡Las contribuciones son bienvenidas!** Puedes:

- 🐛 Reportar bugs, errores ortográficos o fallos gramaticales.
- ®️ Añadir nuevos caracteres, glifos y símbolos a la lista.
- 🌐 Traducir este proyecto a otros idiomas.
- 💡 Mejorar explicaciones y abordar otras propuestas.
- 📝 Mejorar el formato y estilo del código.

Echale un vistazo a las [**pautas de contribución**](../CONTRIBUTING.md) para empezar, y luego anímate en [**abrir un Issue**](https://github.com/soy-daniel-hidalgo/html-character-entities-cheatsheet/issues) o realizar un [**Pull Request**](https://github.com/soy-daniel-hidalgo/html-character-entities-cheatsheet/pulls)!

**(ദ്ദി ˙ᗜ˙ )** Muchas gracias por tomarte el tiempo de leer y apoyar este proyecto.

---

## 📄 Licencias y derechos de autor

Este repositorio está bajo la [Licencia MIT](../LICENSE), la cual se incluye en el directorio raíz de este repositorio. Siéntete libre de usar, adaptar o copiar cualquier parte de este proyecto.

El [logotipo de HTML5](http://www.w3.org/html/logo/) está bajo la licencia Creative Commons Atribución 3.0 — todos son libres de usarlo y reinterpretarlo como crean conveniente.

---

<p align="center">
    <b>⭐ ¡Dale una estrellita al repositorio si te resultó útil! - Te lo agradezco mucho ദ്ദി( • ᴗ - ) ✧ ⭐</b>
</p>
